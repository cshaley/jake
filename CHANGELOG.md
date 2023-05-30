# Changelog

<!--next-version-placeholder-->

## v3.0.1 (2023-05-30)
### Fix

* Handle CWE name suffixed with 'noinfo' ([#129](https://github.com/sonatype-nexus-community/jake/issues/129)) ([`a5d0f11`](https://github.com/sonatype-nexus-community/jake/commit/a5d0f11b9e91e0c00ebd4c227115f38e9eab5eb2))
* CVE-2022-23491 in transitive dependency certifi 2022.5.18.1 by upgrading the version in the lock file. ([`1815487`](https://github.com/sonatype-nexus-community/jake/commit/181548736b0ed0021d78466b2c85413b5b5b6448))
* CVE-2022-23491 in certifi 2022.5.18.1 ([`d964732`](https://github.com/sonatype-nexus-community/jake/commit/d9647329337d5cb47c02eaa884c613228e8b1bec))
* More source file header cleanups ([`261a991`](https://github.com/sonatype-nexus-community/jake/commit/261a9914b019a96c895eb1ad4878d3a0482eb4d5))
* Source file header cleanups ([`6ebf12d`](https://github.com/sonatype-nexus-community/jake/commit/6ebf12d87e6966876575524853247dd50dc9b49f))

### Documentation

* Fix -f switch in the examples ([#126](https://github.com/sonatype-nexus-community/jake/issues/126)) ([`80ac509`](https://github.com/sonatype-nexus-community/jake/commit/80ac50983c6e7e426d84944b31b3d768c7d3517f))

## v3.0.0 (2022-12-02)
### Feature
* Support for all input formats when running jake ddt or jake iq ([#125](https://github.com/sonatype-nexus-community/jake/issues/125)) ([`9a597b5`](https://github.com/sonatype-nexus-community/jake/commit/9a597b59c7f3f042f7188a5cd6a7f6c8c0482f97))

### Fix
* Restore running jake on jake ([`675b359`](https://github.com/sonatype-nexus-community/jake/commit/675b35927a892755ec5fced019646c043ff3d671))

### Breaking
* changed iq -t switch to -st, use common `-f` argument for input file ([`9a597b5`](https://github.com/sonatype-nexus-community/jake/commit/9a597b59c7f3f042f7188a5cd6a7f6c8c0482f97))

## v2.1.1 (2022-06-09)
### Fix
* Removed typo from default value of `--schema-version` argument #117 ([`e9e4764`](https://github.com/sonatype-nexus-community/jake/commit/e9e47649ab87eacdd0a98d8ee9798615d8913fdf))

## v2.1.0 (2022-06-09)
### Feature
* Add support for vulnerability whitelist when running `jake ddt` - thanks @daviskirk! ([`80e1136`](https://github.com/sonatype-nexus-community/jake/commit/80e113620642a032a767bd064ec317a7f19b7de1))

## v2.0.0 (2022-03-10)
### Feature
* Typing as per PEP-561 and other refactors ([#114](https://github.com/sonatype-nexus-community/jake/issues/114)) ([`a0ab7ee`](https://github.com/sonatype-nexus-community/jake/commit/a0ab7eecac96ea9dd1324117651556493247eb98))
* Support for Python 3.10 ([#110](https://github.com/sonatype-nexus-community/jake/issues/110)) ([`671c8c4`](https://github.com/sonatype-nexus-community/jake/commit/671c8c4bb682b4b944568198ecf381818d49f3ac))

### Fix
* Resolve historic oss index caching issues ([`dc03aa9`](https://github.com/sonatype-nexus-community/jake/commit/dc03aa923cf2a8c48d0ad9e7e30cb188fb3a5a96))

### Breaking
* Notion of default schema version has been removed by upstream library and replaced with latest supported schema version ([`e437bb4`](https://github.com/sonatype-nexus-community/jake/commit/e437bb41ddbb84d7844f40b213878c67c071cc23))

## v1.4.5 (2022-02-15)
### Fix
* Pin some upstream dependencies to prevent #112 ([#113](https://github.com/sonatype-nexus-community/jake/issues/113)) ([`8a43e0a`](https://github.com/sonatype-nexus-community/jake/commit/8a43e0af074f797abaddcc0a542b5e08d8a75b36))

## v1.4.4 (2022-02-08)
### Fix
* CWEs are `int` and needed to be stringified ([#102](https://github.com/sonatype-nexus-community/jake/issues/102)) ([`3e15cb1`](https://github.com/sonatype-nexus-community/jake/commit/3e15cb16c037d8bb09eb5c38dbd239dd345f09cc))

## v1.4.3 (2022-02-03)
### Fix
* CWEs not passed as ints to CDX model ([#97](https://github.com/sonatype-nexus-community/jake/issues/97)) ([`6ec49a6`](https://github.com/sonatype-nexus-community/jake/commit/6ec49a6a7d2b22b2535346409ee49fc3cd5f2c8b))

## v1.4.2 (2022-01-31)
### Fix
* Corrected data placement for Vulnerabilities returned from OSS Index when generating an SBOM ([#94](https://github.com/sonatype-nexus-community/jake/issues/94)) ([`eb12286`](https://github.com/sonatype-nexus-community/jake/commit/eb1228602c63784da751749cce14ee9fec9f3d1f))

## v1.4.1 (2022-01-24)
### Fix
* `bom-ref` will always now be populated for Component and Vulnerability - bump of `cyclonedx-python-lib` solves this ([#92](https://github.com/sonatype-nexus-community/jake/issues/92)) ([`df2aad2`](https://github.com/sonatype-nexus-community/jake/commit/df2aad2fa23548e98d2857e2f038e4850067f9b6))

## v1.4.0 (2022-01-13)
### Feature
* Support CycloneDX 1.4 ([#87](https://github.com/sonatype-nexus-community/jake/issues/87)) ([`20c62fc`](https://github.com/sonatype-nexus-community/jake/commit/20c62fcb70d1245e5c31df56ad3d71bc9e7fe0d0))

## v1.3.0 (2022-01-11)
### Feature
* **pre-commit:** Add pre-commit hooks ([#85](https://github.com/sonatype-nexus-community/jake/issues/85)) ([`45f108e`](https://github.com/sonatype-nexus-community/jake/commit/45f108e018925f932768f29855b19342fcec2ac1))

## v1.2.3 (2021-12-22)
### Fix
* Resolved regression when running `jake ddt` where return code != 0 when vulnerabilities discovered ([`8a10e70`](https://github.com/sonatype-nexus-community/jake/commit/8a10e700cea51b649ef7f2271a44e42109264e9a))

## v1.2.2 (2021-12-15)
### Fix
* Removed a number of direct dependencies that are now transitives, or no longer required ([`bcb0a3d`](https://github.com/sonatype-nexus-community/jake/commit/bcb0a3d222c23f88e92fc74c37fd2864e236d8d5))

## v1.2.1 (2021-12-15)
### Fix
* Bumped dependencies to resolve wheel-only installation ([`4ac980d`](https://github.com/sonatype-nexus-community/jake/commit/4ac980d0d7696128e03f982de2dabdfaf7009e03))

## v1.2.0 (2021-12-13)
### Feature
* Replaced `yaspin`, `termcolor` and `terminaltable` with `rich` - see #72, #73, #77 ([`8534ad9`](https://github.com/sonatype-nexus-community/jake/commit/8534ad92acf6b70407492e55ec68ede3190a393b))
* Removed `terminaltables` and replaced with `rich`s table implementation ([`416b03c`](https://github.com/sonatype-nexus-community/jake/commit/416b03c0c844a28512143826453ad956e98abd7c))
* Removed `yaspin` and replaced with `rich` ([`76c4a54`](https://github.com/sonatype-nexus-community/jake/commit/76c4a5451e04c28612ab3c034bbd4a84fa413c94))

### Fix
* Removed f-strings as not required ([`b5b271e`](https://github.com/sonatype-nexus-community/jake/commit/b5b271ed78b97101e9fca2e31b2789540bf66fd4))

## v1.1.5 (2021-12-09)
### Fix
* Bump required version of cyclonedx-python-lib to help lax transitive dependencies ([`f53407f`](https://github.com/sonatype-nexus-community/jake/commit/f53407fb72625420f015db59bb801cc12ab290cf))
* Bump required version of cyclonedx-python-lib to help lax transitive dependencies ([`34e501d`](https://github.com/sonatype-nexus-community/jake/commit/34e501d062da5607f86879e136d1f988de6dd872))

## v1.1.4 (2021-12-07)
### Fix
* Ensure dependencies can be installed from binary packages #72 ([`9e30ca8`](https://github.com/sonatype-nexus-community/jake/commit/9e30ca8d11bc6ee578749686ff3af30b1c805b10))

## v1.1.3 (2021-11-10)
### Fix
* Return exit code up the call stack ([`12caad2`](https://github.com/sonatype-nexus-community/jake/commit/12caad22e2c5bca95d4f2a4bafae5b95b4a7fd2a))

## v1.1.2 (2021-11-10)
### Fix
* Restore "stage" parameter for iq command, for realsies ([`f1d8c64`](https://github.com/sonatype-nexus-community/jake/commit/f1d8c64853c707ccd07dcceb5bd04bffbd4078db))

## v1.1.1 (2021-11-09)
### Fix
* Restore "stage" parameter for iq command ([`01a41da`](https://github.com/sonatype-nexus-community/jake/commit/01a41dae1ca8f13d7f3837f695daa25792f9e834))

## v1.1.0 (2021-10-22)
### Feature
* Add support for conda #66 ([`a3495cb`](https://github.com/sonatype-nexus-community/jake/commit/a3495cb55fe835181ae57a1a48b9ff8cbe7b7415))

## v1.0.1 (2021-10-20)
### Fix
* Update to support returning non-zero exit code when issues found (will return 1) ([`7667bac`](https://github.com/sonatype-nexus-community/jake/commit/7667bacb171803f7963bec12240520985103d06c))

## v1.0.0 (2021-10-18)
### Feature
* Sonatype Nexus IQ Lifecycle analysis is now migrated to using cyclonedx-python-lib ([`214d182`](https://github.com/sonatype-nexus-community/jake/commit/214d1821fa94ff895a2bfa4eac0f6961df093f46))
* Support Poetry for gleaning packages within the current environment to generate an SBOM ([`b9a1e5d`](https://github.com/sonatype-nexus-community/jake/commit/b9a1e5d2f38963a033d102399827c5c4dfe786da))
* Jake's OSS calls now utilising ossindex-lib and cyclonedx-python-lib ([`ec83583`](https://github.com/sonatype-nexus-community/jake/commit/ec83583520aa5ff8180b215b55846ed7a6fd487c))

### Fix
* Additional whitespace removed ([`709f7a2`](https://github.com/sonatype-nexus-community/jake/commit/709f7a2aa752668daba99c04b36ad9b8a6d271f2))
* Runtime tweaks to make it more robust ([`13c9028`](https://github.com/sonatype-nexus-community/jake/commit/13c902838008377e11e4c47ed619401776b8f782))
* Typos noted as updating documentation ([`0d65116`](https://github.com/sonatype-nexus-community/jake/commit/0d65116a17757b1ccf4c73bc463ee677eef0d5ff))

### Breaking
* `jake` has been re-written in large part to consume two new external libraries: - `cyclonedx-python-lib` which gives `jake` ability to more easily consume your depenedencies in a variety of manners (environment, Pipfile.lock, poetry.lock, requirements.txt) and support output in both JSON and XML at different schema versions - `ossindex-lib`: most of the functionallity for talking to OSS Index that was in `jake` has been externalised to this library to allow others to consume it ([`e11cb20`](https://github.com/sonatype-nexus-community/jake/commit/e11cb208c215169d6ce24fa8898a5aa2402d8791))

## v0.2.77 (2021-07-06)
### Fix
* CVE-2021-33503 in urllib3 == 1.26.4 ([#62](https://github.com/sonatype-nexus-community/jake/issues/62)) ([`9dfbb1c`](https://github.com/sonatype-nexus-community/jake/commit/9dfbb1c18831a1456803299e2f98a95ba95ea2b8))

## v0.2.76 (2021-06-29)
### Fix
* "ModuleNotFoundError: No module named 'typing_extensions'", occurring in 'python3.7/site-packages/tinydb/queries.py", line 28' on Jenkins CI ([#61](https://github.com/sonatype-nexus-community/jake/issues/61)) ([`a747750`](https://github.com/sonatype-nexus-community/jake/commit/a7477505a0e6d1b198461a75ef8d755cc37dfe12))

## v0.2.75 (2021-05-25)


## v0.2.74 (2021-05-25)


## v0.2.73 (2021-05-25)


## v0.2.72 (2021-05-13)
### Fix
* Inline targets help changes ([#58](https://github.com/sonatype-nexus-community/jake/issues/58)) ([`c146a7d`](https://github.com/sonatype-nexus-community/jake/commit/c146a7d87e0859040b01278de8a2d09eb9b8b1cb))

## v0.2.71 (2021-05-13)
### Fix
* #49 allow newer version of dependencies ([#57](https://github.com/sonatype-nexus-community/jake/issues/57)) ([`15553d4`](https://github.com/sonatype-nexus-community/jake/commit/15553d43932feca9978931734cf70c655158417d))

## v0.2.70 (2021-04-07)
### Fix
* CVE-2020-14343 in PyYAML==5.3.1 ([`11dc3c9`](https://github.com/sonatype-nexus-community/jake/commit/11dc3c90a2df876e2cda02be33a38c5f2a0c3fc4))

## v0.2.69 (2021-03-25)
### Fix
* CVE-2021-28957 in lxml==4.6.2 ([`6d4373c`](https://github.com/sonatype-nexus-community/jake/commit/6d4373cd8fe320a17d3f8ca95208a0d5b38888ee))

## v0.2.68 (2021-03-23)


## v0.2.67 (2021-03-18)


## v0.2.66 (2021-02-11)


## v0.2.65 (2021-01-27)


## v0.2.64 (2020-12-17)


## v0.2.63 (2020-12-17)


## v0.2.62 (2020-12-17)


## v0.2.61 (2020-12-17)


## v0.2.60 (2020-12-16)


## v0.2.59 (2020-12-09)
### Fix
* Resolve vulnerability: CVE-2020-27783 in lxml ([`7526728`](https://github.com/sonatype-nexus-community/jake/commit/7526728623e102fb75fad30eb82be8824abbdf39))

## v0.2.58 (2020-12-07)


## v0.2.57 (2020-11-12)


## v0.2.56 (2020-11-12)


## v0.2.55 (2020-11-12)


## v0.2.54 (2020-11-12)


## v0.2.53 (2020-11-12)


## v0.2.52 (2020-11-12)


## v0.2.51 (2020-11-11)


## v0.2.50 (2020-11-09)

