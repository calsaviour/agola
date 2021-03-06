## Changelog

### v0.4.0

- gateway/runservice: add api to delete step logs                                            [#157](https://github.com/agola-io/agola/pull/157)
- *: write and flush header on log handlers (@sgotti)                                        [#180](https://github.com/agola-io/agola/pull/180)
- runservice: improve errors in logsHandler (@sgotti)                                        [#179](https://github.com/agola-io/agola/pull/179)
- runservice: use etcd mutex TryLock on fetching (@sgotti)                                   [#177](https://github.com/agola-io/agola/pull/177)
- gateway: add api to get log status (@camandel)                                             [#175](https://github.com/agola-io/agola/pull/175)
- *: use etcd mutex TryLock (@sgotti)                                                        [#176](https://github.com/agola-io/agola/pull/176)
- datamanager: skip already applied wals in writeDataSnapshot (@sgotti)                      [#167](https://github.com/agola-io/agola/pull/167)
- readdb: improve HandleEvents goroutine exiting (@sgotti)                                   [#172](https://github.com/agola-io/agola/pull/172)
- datamanager tests: increase etcd waitdown timeout (@sgotti)                                [#174](https://github.com/agola-io/agola/pull/174)
- *: improve error handling (@sgotti)                                                        [#169](https://github.com/agola-io/agola/pull/169)
- objectstorage: use a single package (@sgotti)                                              [#170](https://github.com/agola-io/agola/pull/170)
- datamanager: refactor ReadWal (@sgotti)                                                    [#168](https://github.com/agola-io/agola/pull/168)
- datamanager: check wal previouswalsequence is correct in initEtcd (@sgotti)                [#165](https://github.com/agola-io/agola/pull/165)
- datamanager: don't create ost wal checkpointed files (@sgotti)                             [#164](https://github.com/agola-io/agola/pull/164)
- datamanager: clean old data files (@sgotti)                                                [#160](https://github.com/agola-io/agola/pull/160)
- datamanager: fix index creation on multiple data files (@sgotti)                           [#163](https://github.com/agola-io/agola/pull/163)
- services: check config only for enabled services (@camandel)                               [#162](https://github.com/agola-io/agola/pull/162)
- datamanager: add data sequence to data file name (@sgotti)                                 [#158](https://github.com/agola-io/agola/pull/158)
- sequence: add tests for String and Parse methods (@sgotti)                                 [#159](https://github.com/agola-io/agola/pull/159)
- go.mod: update dependencies (@sgotti)                                                      [#150](https://github.com/agola-io/agola/pull/150)
- run config: add tty option for run steps (@camandel)                                       [#149](https://github.com/agola-io/agola/pull/149)
- README: issue link points to templates (@camandel)                                         [#156](https://github.com/agola-io/agola/pull/156)
- objectstorage: add WriteObject tests (@sgotti)                                             [#155](https://github.com/agola-io/agola/pull/155)
- objectstorage: return object size in objectinfo (@sgotti)                                  [#154](https://github.com/agola-io/agola/pull/154)
- objectstorage posix: use limitreader only when size is specified. (@sgotti)                [#153](https://github.com/agola-io/agola/pull/153)
- objectstorage s3: use limitreader in write object (@sgotti)                                [#152](https://github.com/agola-io/agola/pull/152)

### v0.3.0

- gitea: use GetRepoRefs instead of GetRepoRef (@sgotti)                                     [#146](https://github.com/agola-io/agola/pull/146)
- when: fix typo in tag matching (@sgotti)                                                   [#147](https://github.com/agola-io/agola/pull/147)
- cmd: add run create command (@sgotti)                                                      [#144](https://github.com/agola-io/agola/pull/144)
- gateway: fix project create run http method (@sgotti)                                      [#143](https://github.com/agola-io/agola/pull/143)
- docker: mount multiple volumes (@camandel)                                                 [#142](https://github.com/agola-io/agola/pull/142)
- gitsources: don't set branch value when in a pull request (@sgotti)                        [#140](https://github.com/agola-io/agola/pull/140)
- when: match only the current ref type (@sgotti)                                            [#139](https://github.com/agola-io/agola/pull/139)
- \*: implement ability to add tmpfs volumes to containers (@sgotti)                         [#136](https://github.com/agola-io/agola/pull/136)
- cmd: add version command (@camandel)                                                       [#135](https://github.com/agola-io/agola/pull/135)
- datamanager: remove some logs from tests (@sgotti)                                         [#134](https://github.com/agola-io/agola/pull/134)
- cmd: add completion command (@camandel)                                                    [#133](https://github.com/agola-io/agola/pull/133)
- cmd: add project group delete command (@sgotti)                                            [#132](https://github.com/agola-io/agola/pull/132)
- cmd: add project group update command (@sgotti)                                            [#131](https://github.com/agola-io/agola/pull/131)
- gateway: add parentRef field to project group update api (@sgotti)                         [#130](https://github.com/agola-io/agola/pull/130)
- configstore: implement project group move (@sgotti)                                        [#128](https://github.com/agola-io/agola/pull/128)
- configstore: disable root project group deletion (@sgotti)                                 [#129](https://github.com/agola-io/agola/pull/129)
- cmd: add project update command (@sgotti)                                                  [#123](https://github.com/agola-io/agola/pull/123)
- tests: wait gitea ready (@sgotti)                                                          [#127](https://github.com/agola-io/agola/pull/127)
- gateway: add parentRef field to project update api (@sgotti)                               [#122](https://github.com/agola-io/agola/pull/122)
- cmd: fix version output (@camandel)                                                        [#126](https://github.com/agola-io/agola/pull/126)
- Add github issue templates (@sgotti)                                                       [#125](https://github.com/agola-io/agola/pull/125)
- configstore: implement project move (@sgotti)                                              [#121](https://github.com/agola-io/agola/pull/121)
- cmd: fix typos in online help (@camandel)                                                  [#124](https://github.com/agola-io/agola/pull/124)
- cli: add secret/variable list subcommand (@camandel)                                       [#118](https://github.com/agola-io/agola/pull/118)
- config: add clone options (@camandel)                                                      [#120](https://github.com/agola-io/agola/pull/120)
- gateway: api implement get secrets removeoverridden (@sgotti)                              [#119](https://github.com/agola-io/agola/pull/119)
- skip run with special commit (@camandel)                                                   [#90](https://github.com/agola-io/agola/pull/90)
- executor: add missing mutex unlock (@sgotti)                                               [#117](https://github.com/agola-io/agola/pull/117)
- gateway: run api return more step data (@sgotti)                                           [#116](https://github.com/agola-io/agola/pull/116)
- runservice: save step exitstatus in run. (@sgotti)                                         [#115](https://github.com/agola-io/agola/pull/115)
- runservice: don't save executor task data in etcd (@sgotti)                                [#113](https://github.com/agola-io/agola/pull/113)
- runservice: add run workspace cleaner (@sgotti)                                            [#109](https://github.com/agola-io/agola/pull/109)
- executor: set the container exec user in every step (@sgotti)                              [#112](https://github.com/agola-io/agola/pull/112)
- runconfig: set task default shell (@sgotti)                                                [#111](https://github.com/agola-io/agola/pull/111)
- runservice: remove run step user (@sgotti)                                                 [#110](https://github.com/agola-io/agola/pull/110)
- \*: update to go 1.13 (@sgotti)                                                            [#105](https://github.com/agola-io/agola/pull/105)
- gitserver: don't return http response/error when calling external git process (@sgotti)    [#103](https://github.com/agola-io/agola/pull/103)
- util: Fix PathList output when path ends with slashes (@sgotti)                            [#102](https://github.com/agola-io/agola/pull/102)

### v0.2.0

- agola run: update to agola-web v0.2.0 (@sgotti)                                            [#100](https://github.com/agola-io/agola/pull/100)
- types: use a global When type (@sgotti)                                                    [#99](https://github.com/agola-io/agola/pull/99)
- agola run: update to agola-web v0.1.2 (@sgotti)                                            [#95](https://github.com/agola-io/agola/pull/95)
- README.md: update screenshots (@sgotti)                                                    [#96](https://github.com/agola-io/agola/pull/96)
- agola run: build images and push them when on a v.\* tag (@sgotti)                         [#94](https://github.com/agola-io/agola/pull/94)
- runservice: fix get tasks to run (@sgotti)                                                 [#93](https://github.com/agola-io/agola/pull/93)
- tests: add wait function in place of sleep (@sgotti)                                       [#92](https://github.com/agola-io/agola/pull/92)
- cmd: fix variable create/update (@sgotti)                                                  [#91](https://github.com/agola-io/agola/pull/91)
- update example in devel doc (@camandel)                                                    [#89](https://github.com/agola-io/agola/pull/89)
- config: fix check on task and parents with common deps (@sgotti)                           [#88](https://github.com/agola-io/agola/pull/88)
- userdirectrun: add options to define variables (@sgotti)                                   [#86](https://github.com/agola-io/agola/pull/86)
- Dockerfile: update to debian buster (@sgotti)                                              [#85](https://github.com/agola-io/agola/pull/85)
- executor: listen on wildcard address (@sgotti)                                             [#84](https://github.com/agola-io/agola/pull/84)
- config: add run when field (@sgotti)                                                       [#78](https://github.com/agola-io/agola/pull/78)
- userdirectrun: allow setting destination branch/tag/ref (@sgotti)                          [#83](https://github.com/agola-io/agola/pull/83)
- tests: test also clone step (@sgotti)                                                      [#82](https://github.com/agola-io/agola/pull/82)
- docker driver: use fixed client api version (@sgotti)                                      [#81](https://github.com/agola-io/agola/pull/81)
- docker driver: use toolbox exec (@sgotti)                                                  [#80](https://github.com/agola-io/agola/pull/80)
- \*: export clients and related types (@sgotti)                                             [#77](https://github.com/agola-io/agola/pull/77)
- configstore: move configstore types inside configstore package (@sgotti)                   [#76](https://github.com/agola-io/agola/pull/76)
- util: remove time.go (@sgotti)                                                             [#75](https://github.com/agola-io/agola/pull/75)
- executor: set task endTime when marking as failed (@sgotti)                                [#71](https://github.com/agola-io/agola/pull/71)
- executor: fix typo in setting task endTime when setup failed (@sgotti)                     [#70](https://github.com/agola-io/agola/pull/70)
- runservice: fix/improve executor delete logic (@sgotti)                                    [#69](https://github.com/agola-io/agola/pull/69)
- runservice: maintenance/export/import (@sgotti)                                            [#68](https://github.com/agola-io/agola/pull/68)
- configstore: maintenance/export/import (@sgotti)                                           [#67](https://github.com/agola-io/agola/pull/67)
- util: use context in backoff (@sgotti)                                                     [#66](https://github.com/agola-io/agola/pull/66)
- readdb: close and open readdb on Run (@sgotti)                                             [#65](https://github.com/agola-io/agola/pull/65)
- \*: use sleep timer in loops (@sgotti)                                                     [#64](https://github.com/agola-io/agola/pull/64)
- db: use context functions (@sgotti)                                                        [#62](https://github.com/agola-io/agola/pull/62)
- datamanager: implement import/export (@sgotti)                                             [#63](https://github.com/agola-io/agola/pull/63)
- datamanager: implement maintenance mode (@sgotti)                                          [#61](https://github.com/agola-io/agola/pull/61)
- go mod: update golang.org/x/xerrors (@sgotti)                                              [#60](https://github.com/agola-io/agola/pull/60)
- db: retry on sqlite locked error (@sgotti)                                                 [#59](https://github.com/agola-io/agola/pull/59)
- readdb: fix deadlock in Run method (@sgotti)                                               [#58](https://github.com/agola-io/agola/pull/58)
- runservice: stop run also if result is not set (@sgotti)                                   [#57](https://github.com/agola-io/agola/pull/57)
