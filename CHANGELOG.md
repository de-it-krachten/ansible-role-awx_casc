# [1.7.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.6.0...v1.7.0) (2025-04-08)


### Features

* Add support for workflow recreation ([327f78c](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/327f78cde178f99e8950da24d2cb2385fdc7d284))

# [1.6.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.5.0...v1.6.0) (2024-12-29)


### Features

* Update supported platforms & CI ([ec2b115](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/ec2b1159201509bbb9417cc4560a4e4708f6933e))

# [1.5.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.4.0...v1.5.0) (2024-09-27)


### Features

* Add support for workflow templates using jinja vars ([3a90b6e](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/3a90b6eaef56dd95283b7e9356c2c161a4a4be0f))
* group | Add support for variable template ([dff5946](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/dff5946c3285c0eb40b0a2a955e17fc6db1de98c))
* host | Add support for variable template ([f8372cb](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/f8372cbe604e4ab065fbbf1b71de5712760abe2e))
* inventory | Add support for variable template ([51edcd2](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/51edcd25146117a4183cfaaeb864b87a84470268))

# [1.4.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.3.1...v1.4.0) (2024-06-03)


### Bug Fixes

* Read user password from external file ([d21a7e9](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/d21a7e91ae4daf088358c221a0ef7bdd278ae270))


### Features

* Add support for Ubuntu 24.04 LTS + Fedora 40 ([ebfd739](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/ebfd739c7eacb0ad6a048b174234b27b44cc15ad))

## [1.3.1](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.3.0...v1.3.1) (2024-04-11)


### Bug Fixes

* Fix wrong variables for vars/inputs ([43e1e4c](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/43e1e4c498374e12c3592974757a42f1e201c078))

# [1.3.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.2.1...v1.3.0) (2023-11-08)


### Bug Fixes

* Add support for inline variables/extra-vars ([2d0cbbc](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/2d0cbbcb4e8048d21c8f006057e67f7c9e783dcd))


### Features

* Add support for variables/extra-vars in yaml format ([49b487f](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/49b487f828f0e9967bafe89e7dd59eb55f14c620))

## [1.2.1](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.2.0...v1.2.1) (2023-09-22)


### Bug Fixes

* Retrieve token when running in check-mode ([1bdea64](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/1bdea640dd39f68d583e3c9ced4af99e18d5e14d))

# [1.2.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.1.0...v1.2.0) (2023-09-20)


### Bug Fixes

* Add optional skipping of assigning hosts to groups ([3a8930a](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/3a8930aa34dfe2597ba7fbf8f58edefa673e31df))
* Change loop/label for latest ansible ([8f375d2](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/8f375d22391581870adeb14e499e8b72e4b7406e))


### Features

* Add support for AWX execution environments ([97f29db](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/97f29dbdd027f1cb63590c1440af2d068b660c94))
* Update supported platforms & CI ([aaffbfc](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/aaffbfcd26a7d2040c01af6c5ca2f5e4fa375d7f))

# [1.1.0](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.0.3...v1.1.0) (2023-05-06)


### Bug Fixes

* Add support for credential input ([0d20191](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/0d20191548421cb795a7b387a04656a6dba046f9))
* Fix issues encountered when creating from scratch ([90b1592](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/90b1592187e492f0434bf0f6b31b1c843449471c))
* Implement missing parameters for all modules ([3dadd76](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/3dadd766af5aaf09bf219cd19538112e315764a0))


### Features

* Add optional check for host presense in DNS ([911702a](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/911702a03711ffeb7160b1286fb17acc95a00e9f))

## [1.0.3](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.0.2...v1.0.3) (2022-11-10)


### Bug Fixes

* Ignoring errors on 'projects' & 'job_templates' ([d1920fd](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/d1920fd1ef2dfd011e642d9a82a9c02b8450049f))

## [1.0.2](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.0.1...v1.0.2) (2022-10-24)


### Bug Fixes

* change default import behaviour to skip updates on encrypted values ([6ad90e0](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/6ad90e0183ca42eb197b7769141e6e3b5c89d83d))

## [1.0.1](https://github.com/de-it-krachten/ansible-role-awx_casc/compare/v1.0.0...v1.0.1) (2022-10-24)


### Bug Fixes

* Add missing resource type 'organizations' ([b33d281](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/b33d2817e64860481154d8a3c8c8d3b925314bd3))

# 1.0.0 (2022-10-20)


### Features

* Initial release ([31c1247](https://github.com/de-it-krachten/ansible-role-awx_casc/commit/31c1247c657bb890a615a9407659ecd2410f3545))
