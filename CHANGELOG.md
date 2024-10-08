# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).

## [Unreleased](https://github.com/RCIC-UCI-Public/slurm-admix/compare/2.0...HEAD)

### Commits

- add slurm 24.05.03 [`8d2e55e`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/8d2e55e059562ff0554b1d92c6c41d52b7342715)
- Added more debugging info and fixed the sbank deposit issue. [`d499723`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/d49972316ac7293baf5f5e4f727fbd7054e81635)
- sbank Release 6: modified to tracking billing instead of cpu time [`d5eb7d9`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/d5eb7d9608b2aadfb75f684ccacefb3ecce80e89)
- Remove some items that we don't need [`ad55c94`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ad55c94447d13eafade2e690f868251e848d0401)
- add version info for munge and mysql-connector [`e1fcb9c`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/e1fcb9cc133d420ed20102f6f2cdf2acb2ee6d54)
- original spec file in slurm-bank creates namesake RPM. need to keep this yaml [`700d0e9`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/700d0e93442789eecae789d728bedb306dfa3ba6)
- mv building slurm-bank and slurm-jobarchive to build area [`6b0066c`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/6b0066c1555d3ddf9a484eea21c40e3427b7e12f)
- rename to keep name consistency [`62df95a`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/62df95aed652f47278d9807468501a153fcc83ef)
- add on patch to increase version of the rpm release [`eed4624`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/eed462478a7fad7ad4db7f3c31204fd96350987b)
- add auto-changelog generated CHANGELOG.md [`e98daa1`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/e98daa17e6216fa41fa720038fe367914eda68c2)

## 2.0 - 2023-08-09

### Commits

- create a set for slurm v.23.02.3 [`b70dfba`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/b70dfbabe1febb60f6ffc7cdf68ac6db66ee18ff)
- add source distro for slurm 23.02.3.1 [`9f27277`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/9f27277e8acace2ccf0666a450bd50b547453947)
- add perl-ExtUtils-MakeMaker to bootstarp/ is required to build slurm rpms [`5a534ab`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/5a534ab596db5b987e4f99bf02f9c77bf04ae9c8)
- patch sbank to have correct first line [`7ea8356`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/7ea83560510403eca1e659e22d7deba0254ca5fc)
- Patch _sbank-balance.pl to print per user account limits and respect them [`87fec17`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/87fec17a5c20b1ef111a506c9f5a3223608a5958)
- More robust way of getting just the SU allocation for the account [`bd6a0d0`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/bd6a0d0ee89ca92126875ee632e661242ebeb37d)
- Patch slurm-bank to ignore cpu limits on individuals within a lab [`3a92b39`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/3a92b39bc5ab1a64b0e6bf1ce989425db2e2e7cd)
- add vendor into RPM info header. The original spec file from SLURM [`00e5f08`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/00e5f08be81467836a85d18bc07b533d8fc11117)
- separate variables into lines [`be727ab`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/be727abd79f20b0ffbd4ff80ec9137fc3624fdd5)
- rm unneeded [`51d36df`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/51d36dfae7cc32a2d3eeebcb30bf00f1501a1e68)
- patch so that /etc/clsutershell and its files are not installed [`ce5a9ed`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ce5a9ed02c943e641615d075dcc9072ce10c06a8)
- add openblas and cython as dependencies so the RPM install will [`be50438`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/be504384562fdf2b6165c47f737de6036e42294c)
- add SRPMS and *pkg [`a03e2d8`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/a03e2d8dcf407f067a8be76ff6f28a0136a8ab20)
- add pandas.yaml, mysql-connector.yaml,  clustershell.yaml, cython.yaml [`298ff21`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/298ff2113e39c7b0e8f68315c7047e465472c4ef)
- update slurm to 22.05.3 [`bf960a5`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/bf960a5923573e2cc7639ab40b440291768f03cc)
- add to listing of slurm created packages slurm-libpmi and slurm-perlapi [`c212cb4`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/c212cb4d4208324b6b5365d1ed5f24ee4bc2fc22)
- typo and shorten lines [`0c20ae9`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/0c20ae9e48e67d5c404bba70ae1e7cc76514e493)
- add slurm-bank [`52465b7`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/52465b7ffe7ba00766321ef3f9a457c383081629)
- rm non-existing package [`d6502a1`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/d6502a12781f7fd46e31ee52e5da7fc56bb51eb1)
- add .gitignore [`9eab7cd`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/9eab7cd66bd5a9b02c78ccecdcfd38882de7189f)
- update info about job arhiver [`ff4cdc1`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ff4cdc1861dcc6cbe9f3ebe07cd547d5486e3fff)
- add slurm 19.05.3-2 patch for reference [`ccb83cc`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ccb83ccd4fa60e7fbd745c66e0319567a44b4cf1)
- add slurm distro for v 19.05.03-2, 20.11.9, 22.05.2 and for job-arhiver [`3056947`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/3056947aae9a799bc2db23bcf3ce083c72d5e9b3)
- build slurm-jobarchive RPM [`49d7888`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/49d7888f0bee74f2da39eea56e57b6e2be2e6f29)
- build RPMS for slurm for versions 19.05.3-2, 20.11.9, 22.05.2 [`1b4b767`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/1b4b76791deaf0457b408a88dbe22bcd3e400ee8)
- add munge and slurm tarballs [`1f97107`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/1f97107fa870b89bcf6564dc6035e419bce7019e)
- Initial Check in for build of slurm/munge RPMS [`c872d90`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/c872d905ee494fdf5089578e02e62785e80e7369)

<!-- auto-changelog-above -->
# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).

## [Unreleased](https://github.com/RCIC-UCI-Public/slurm-admix/compare/2.0...HEAD)

## 2.0 - 2023-08-09

### Commits

- create a set for slurm v.23.02.3 [`b70dfba`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/b70dfbabe1febb60f6ffc7cdf68ac6db66ee18ff)
- add source distro for slurm 23.02.3.1 [`9f27277`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/9f27277e8acace2ccf0666a450bd50b547453947)
- add perl-ExtUtils-MakeMaker to bootstarp/ is required to build slurm rpms [`5a534ab`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/5a534ab596db5b987e4f99bf02f9c77bf04ae9c8)
- patch sbank to have correct first line [`7ea8356`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/7ea83560510403eca1e659e22d7deba0254ca5fc)
- Patch _sbank-balance.pl to print per user account limits and respect them [`87fec17`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/87fec17a5c20b1ef111a506c9f5a3223608a5958)
- More robust way of getting just the SU allocation for the account [`bd6a0d0`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/bd6a0d0ee89ca92126875ee632e661242ebeb37d)
- Patch slurm-bank to ignore cpu limits on individuals within a lab [`3a92b39`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/3a92b39bc5ab1a64b0e6bf1ce989425db2e2e7cd)
- add vendor into RPM info header. The original spec file from SLURM [`00e5f08`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/00e5f08be81467836a85d18bc07b533d8fc11117)
- separate variables into lines [`be727ab`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/be727abd79f20b0ffbd4ff80ec9137fc3624fdd5)
- rm unneeded [`51d36df`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/51d36dfae7cc32a2d3eeebcb30bf00f1501a1e68)
- patch so that /etc/clsutershell and its files are not installed [`ce5a9ed`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ce5a9ed02c943e641615d075dcc9072ce10c06a8)
- add openblas and cython as dependencies so the RPM install will [`be50438`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/be504384562fdf2b6165c47f737de6036e42294c)
- add SRPMS and *pkg [`a03e2d8`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/a03e2d8dcf407f067a8be76ff6f28a0136a8ab20)
- add pandas.yaml, mysql-connector.yaml,  clustershell.yaml, cython.yaml [`298ff21`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/298ff2113e39c7b0e8f68315c7047e465472c4ef)
- update slurm to 22.05.3 [`bf960a5`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/bf960a5923573e2cc7639ab40b440291768f03cc)
- add to listing of slurm created packages slurm-libpmi and slurm-perlapi [`c212cb4`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/c212cb4d4208324b6b5365d1ed5f24ee4bc2fc22)
- typo and shorten lines [`0c20ae9`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/0c20ae9e48e67d5c404bba70ae1e7cc76514e493)
- add slurm-bank [`52465b7`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/52465b7ffe7ba00766321ef3f9a457c383081629)
- rm non-existing package [`d6502a1`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/d6502a12781f7fd46e31ee52e5da7fc56bb51eb1)
- add .gitignore [`9eab7cd`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/9eab7cd66bd5a9b02c78ccecdcfd38882de7189f)
- update info about job arhiver [`ff4cdc1`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ff4cdc1861dcc6cbe9f3ebe07cd547d5486e3fff)
- add slurm 19.05.3-2 patch for reference [`ccb83cc`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/ccb83ccd4fa60e7fbd745c66e0319567a44b4cf1)
- add slurm distro for v 19.05.03-2, 20.11.9, 22.05.2 and for job-arhiver [`3056947`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/3056947aae9a799bc2db23bcf3ce083c72d5e9b3)
- build slurm-jobarchive RPM [`49d7888`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/49d7888f0bee74f2da39eea56e57b6e2be2e6f29)
- build RPMS for slurm for versions 19.05.3-2, 20.11.9, 22.05.2 [`1b4b767`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/1b4b76791deaf0457b408a88dbe22bcd3e400ee8)
- add munge and slurm tarballs [`1f97107`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/1f97107fa870b89bcf6564dc6035e419bce7019e)
- Initial Check in for build of slurm/munge RPMS [`c872d90`](https://github.com/RCIC-UCI-Public/slurm-admix/commit/c872d905ee494fdf5089578e02e62785e80e7369)
