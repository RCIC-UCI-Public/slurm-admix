# slurm-admix
A collection of slurm RPMS

## Slurm builder

A wrapper script to use download slurm distro file and build RPMs via rpmbuild
using the distro spec file.

1. version  19.05.3-2 

   This is the current slurm version on CentOS7 HPC3
   Due to a security vulnerability (CVE-2022-29500), all versions of Slurm prior to 
   21.08.8 or 20.11.9 are no longer available for download. See https://www.schedmd.com/archives.php

   Download from git  then patch and repack as bz2 archive:
   ```bash
   wget https://github.com/SchedMD/slurm/archive/refs/tags/slurm-19-05-3-2.tar.gz
   tar xzvf slurm-19-05-3-2.tar.gz 
   mv slurm-slurm-19-05-3-2/ slurm-19.05.3-2
   cd slurm-19.05.3-2
   cp slurm.spec slurm.spec.orig
   vim slurm.spec
   diff -Naur slurm.spec.orig slurm.spec > ../slurm-19.05.3-2.spec.patch
   cd ..
   tar cvf slurm-19.05.3-2.tar slurm-19.05.3-2
   bzip2 slurm-19.05.3-2.tar
   mv slurm-19.05.3-2.tar.bz2 ../sources
   ```

   Use resulting slurm-19.05.3-2.tar.bz2 for building the RPMS.
   For this version need to set *slurm_tag* in versions-19.yaml
   because of the distro's slurm.spec file and other files dependency on 
   this specific versionsing "19.05.3-2". Using "-" in version does not work
   when building RPMs as "-" is an illegal character in version.

1. version  20.11.9  
   
   build a temp RPM set when transitioning from slurm v.19 to slurm v.22

1. version  22.05.2  
   
    slurm version for move to Rocky 8

## slurm-jobarhive 

Create an RPM with a slurm job archiver binary and a service file 

This following info is added to the distro README (new) file:

Orioginal code is in https://github.com/nauhpc/job_archive
A version as of commit 2725c0432e8fc24d42734bade82a9dd58144e16f
was checked out on slurm headnode, compiled and used on (centOS7) HPC3. 
There were a few edits to the source cpp file. 

The following variables are hard-coded in the job_archive.cpp per slurm headnode configiuration:
string srcSpoolHashPath  - local slurm spool directory
string targDestPath      - local submit scipts archiveng direcotry

Copy source files from slurm-i14, apply patches, crete slurm-jobarchive-1.0.tar.gz

Changelog 

1. patch for CentOS7 was` applied July 2022
   appliy patch to job_archive.cpp (contents are in job_archive.cpp.patch)
   This patch  removes a lasty null character that is put by slurm 
   in submit file and is copied by the slurm job archive binary. 
   job_archive.cpp.patch is saved for a reference, no need to apply.

1. patch for CentOS8 was applied Aug 2022
   apply a patch to HelperFn.h to tighten permissions to the created 
   archived files. Originally the permissions were set open to anyone. 
   This worked when job archive was run form a command line as root. 
   When run as a slurm user as a service created directories are searchable by all.
   See file for details.

## slurm-bank

The old repo is checked out from https://github.com/jcftang/slurm-bank.git
commit 60dbd9097865e0cbac224d007bee66f0c68d86a5 (HEAD -> master, origin/master, origin/HEAD)
Date:   Fri Oct 26 13:35:35 2018 +0800

Create a distro file and assigne a version specified in the repo's VERSION file.

```bash
git clone https://github.com/jcftang/slurm-bank.git
vim slurm-bank/slurm-bank.spec
mv slurm-bank/ slurm-bank-1.4.2
tar czf slurm-bank-1.4.2.tar.gz --exclude slurm-bank-1.4.2/.git --exclude slurm-bank-1.4.2/.gitignore slurm-bank-1.4.2/
mv slurm-bank-1.4.2.tar.gz ../sources
```

Edits in slurm-bank.spec file are minimal:

```bash
diff slurm-bank/slurm-bank.spec.orig  slurm-bank.old/slurm-bank.spec
14,15c14,15
< BuildRequires:  perl, bash, rsync, make
< Requires:       slurm >= 2.2.0, perl, bash
---
> BuildRequires:  bash, rsync, make
> Requires:       slurm >= 2.2.0, bash
```
