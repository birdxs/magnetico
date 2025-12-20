## 0.1.0 (2025-12-20)


### ⚠ BREAKING CHANGES

* review the logic related to the operational flags
* introduce the ability to use a configuration file
* allow user supplied ports for bootstrap nodes
* merge the magneticod and magneticow binaries
* do not try to integrate with upnp
* **mainline:** stats should be tracked in a separate struct
* **persistence:** drop support for stdout

### Features

* add api endpoint to get total count of torrents based on query keyword ([bd5c138](https://github.com/birdxs/magnetico/commit/bd5c138bba29c9e1b7430fc1fa82f4b2320c91e2))
* add arm64 to multi-platform container builds ([4a09971](https://github.com/birdxs/magnetico/commit/4a09971b9f9ecd26c7dc3f40c5290b0f6a6138c3))
* add validation for filter-nodes-cidrs during parsing ([50e7717](https://github.com/birdxs/magnetico/commit/50e77170a178e0c588c16cc3f19368896e06100b))
* allow user supplied ports for bootstrap nodes ([774ed20](https://github.com/birdxs/magnetico/commit/774ed206dd7c473a4004083b697f1e4c011b4f88))
* **ci:** commit-lint for PR ([9e30f1b](https://github.com/birdxs/magnetico/commit/9e30f1b3f186e0678b2ae41566ffe1ad4d7b4498))
* **ci:** enable codecov ([f7b8fa6](https://github.com/birdxs/magnetico/commit/f7b8fa6a77704edefeddbba3869a6e4b8f9f353a))
* **ci:** publish multi-platform executables in releases ([89f7f02](https://github.com/birdxs/magnetico/commit/89f7f020b6ccb20f80b54127d41c5004d542e5b1))
* **ci:** publish on ghcr with the next tag ([8cd1af8](https://github.com/birdxs/magnetico/commit/8cd1af82a9de285355962a3817d8836e0ef77aaf))
* **ci:** test with go v1.21 && go v1.22 ([2493da3](https://github.com/birdxs/magnetico/commit/2493da30b2799edf85c4f28f37e97e3aac6e05de))
* **ci:** use dependabot for `/torrent` ([84b16f8](https://github.com/birdxs/magnetico/commit/84b16f8c85d83258fb0a8282b0a319bcd084e03c))
* **config:** Allows the torrent client to customise the client identity and connection config ([6ab65a4](https://github.com/birdxs/magnetico/commit/6ab65a49a8a72dea1a28968b2ab42a85fd4566ec))
* **dht:** crawl only specified ip ranges ([acb1913](https://github.com/birdxs/magnetico/commit/acb19137b5776343b8fa087615ee95ab4436eb70))
* **dht:** implement NewSampleInfohashesResponse and onSampleInfohashesQuery ([6d69021](https://github.com/birdxs/magnetico/commit/6d69021c26526a04855e7d35c0dfcc138172b02e))
* **dht:** implement support for additional mainline methods ([db977b7](https://github.com/birdxs/magnetico/commit/db977b7dcfb056e7f20604283f7a2a4b3c4ff381))
* **dht:** introduce support for the ipv6 krpc protocol ([66fc7b0](https://github.com/birdxs/magnetico/commit/66fc7b098eb3e09021df84dd0dc0e680f4554f73))
* do not try to integrate with upnp ([11360af](https://github.com/birdxs/magnetico/commit/11360af14bba9f20fdd40c2ac1bf24bb7e466c10))
* **docker:** reintroduce a dockerfile ([3abdc72](https://github.com/birdxs/magnetico/commit/3abdc724f31280fb0566e96daceb67f1c85a2f5b))
* flush metrics every minute ([de6001b](https://github.com/birdxs/magnetico/commit/de6001b6fdaaa46f6dab8476813c7439bb3c59a6))
* introduce the ability to use a configuration file ([6eb27c2](https://github.com/birdxs/magnetico/commit/6eb27c2a17f8ff3db92b2e40cc413a4d779c63ea))
* **mainline:** add some missing implementations ([26f6c12](https://github.com/birdxs/magnetico/commit/26f6c12b6cf3afcb8b7e4555671e50f75596fb1f))
* **mainline:** add unit testing for the protocol builder ([930b76b](https://github.com/birdxs/magnetico/commit/930b76b7f3e8efe1702dcd5b780544cce541b017))
* **mainline:** allow user-supplied bootstrap nodes ([05a9ad7](https://github.com/birdxs/magnetico/commit/05a9ad7e1c6f94c5b5deb6e241af48db4a006c7d))
* **mainline:** experimental support for ping / announce_peer ([4a3a91f](https://github.com/birdxs/magnetico/commit/4a3a91f10e4710a0cea9077618494bbf639a7dd6))
* **mainline:** implement the remaining checks ([a7bf9f5](https://github.com/birdxs/magnetico/commit/a7bf9f5a0c3918ccaee04dc5f55d3f900eff8b13))
* **mainline:** parallelize the bootstrap process ([13a4d3c](https://github.com/birdxs/magnetico/commit/13a4d3c79eef10c1aff8552597882415c1b9c211))
* **mainline:** use a udp conn and not a unix socket ([4bda336](https://github.com/birdxs/magnetico/commit/4bda336ee14905bcd67a1ea6808cc3c14d1bc883))
* **mainline:** validate nodes before routing table insertion ([7a433c9](https://github.com/birdxs/magnetico/commit/7a433c98e6677bcef876b9f00a6108bea82064ca))
* merge the magneticod and magneticow binaries ([364d47f](https://github.com/birdxs/magnetico/commit/364d47fd05a18bde84680341c7f7b9fe108c9255))
* **metadata:** add support for message stream encryption ([783dca8](https://github.com/birdxs/magnetico/commit/783dca89fb4ff56ccb6b10f6a4e0e2df3d8acf03))
* **metadata:** add support for Multipath TCP ([e81f3b1](https://github.com/birdxs/magnetico/commit/e81f3b1e4ccdfe0926de070b222a2629859ed7ba))
* **metadata:** add unit testing for `Sink.Drain` ([11f98ad](https://github.com/birdxs/magnetico/commit/11f98ad74ca4ef5ba3fb45b4b62559fc242726cb))
* **metadata:** add unit testing for `Sink.Sink` and `Sink.terminate` ([566b7e4](https://github.com/birdxs/magnetico/commit/566b7e412d5641e0366a6ec5f00647ed38ee3899))
* **metainfo:** add json and mapstructure tags to metainfo structs ([e7a6d67](https://github.com/birdxs/magnetico/commit/e7a6d67beedda8af79e30cbf6827da467dda020c))
* **metainfo:** support for serializing v2 torrent file ([a8c2460](https://github.com/birdxs/magnetico/commit/a8c2460727c2aeb01b16783342651d3606c10794))
* **opflags:** add a flag for the deadline of leeches ([9709b18](https://github.com/birdxs/magnetico/commit/9709b1863381fe0bf440cd4bb16eda99bf40db01))
* **persistence:** add database import functionality ([6f0cfb1](https://github.com/birdxs/magnetico/commit/6f0cfb1141c36b27e5c9c85cbfb990a5e8a478d7))
* **persistence:** add rabbitmq amqp basic support ([24925ba](https://github.com/birdxs/magnetico/commit/24925ba2f5896fffcef183067fa709733b998457))
* **persistence:** add support for the bitmagnet import api ([0a4579d](https://github.com/birdxs/magnetico/commit/0a4579d496ce27f06e17c4d276d28bf8ddcf74f8))
* **persistence:** allows postgres to find torrents by searching for file names ([c81b406](https://github.com/birdxs/magnetico/commit/c81b40677a0ca73ed7865a4774c52e072d709269))
* **persistence:** implement a ZeroMQ interface ([a4654c2](https://github.com/birdxs/magnetico/commit/a4654c2aeafc29e4aae2af3fb9696caebefce172))
* **persistence:** implement database export functionality ([c804674](https://github.com/birdxs/magnetico/commit/c80467425edd3a8da0e9f228e624ab1c38b16a26))
* **persistence:** implement export method for database interfaces ([7a705a6](https://github.com/birdxs/magnetico/commit/7a705a69e08b3c9e968a68f8807533715ddbfae7))
* **persistence:** perform pattern matching without case sensitivity ([b27c8b1](https://github.com/birdxs/magnetico/commit/b27c8b130aef60a134ef99d033d6e6222ff26dbf))
* **persistence:** reintroduce support for sqlite3 ([e276d6f](https://github.com/birdxs/magnetico/commit/e276d6ff7bd8d0d5ead24b7322629ea87c9e61d5))
* **persistence:** support both cgo and non-cgo builds ([96ee524](https://github.com/birdxs/magnetico/commit/96ee524fe213076f02bfb42d35604e90c394cdef))
* remove print BuildFromFilePath ([7d32790](https://github.com/birdxs/magnetico/commit/7d327905fe11903e0040dddb5568b001d05c5d6c))
* **stats:** add a package for logging metrics ([c96820b](https://github.com/birdxs/magnetico/commit/c96820b09179558ba2bfca34d3f879a7571a27a6))
* **stats:** add prometheus exporter for application metrics ([fc12657](https://github.com/birdxs/magnetico/commit/fc126578bce118aba0ee1b19565984973a85ec28))
* **stats:** add pyroscope profiling support ([5d261e1](https://github.com/birdxs/magnetico/commit/5d261e12df1e29445a03e9bc5478729efef2900d))
* **torrent:** replace anacrolix with the embedded torrent ([11cf7d7](https://github.com/birdxs/magnetico/commit/11cf7d703ebefee6fc571c114aaae04d29d2e0bc))
* **torrent:** use bolt in place of sqlite for piece completion ([486ce86](https://github.com/birdxs/magnetico/commit/486ce8696c7505c5943a52a0c8cf785cdc007d57))
* **web:** add count parameter to rss feed ([8e7d2cf](https://github.com/birdxs/magnetico/commit/8e7d2cfdb277aaff814df99e46b13859be72ac65))
* **web:** add new parameters with different semantics to the `torrentstotal` api ([fc60049](https://github.com/birdxs/magnetico/commit/fc60049ad9f4ed417bdb2e186ddb22a270d98127))
* **web:** add redirect for non-root paths and handle invalid methods ([3604006](https://github.com/birdxs/magnetico/commit/360400601ab494a68accb06e455ceac2db060554))
* **web:** add timeout configuration for web interface and apis ([2255959](https://github.com/birdxs/magnetico/commit/225595982cdf094762aabe99d809ca76c1104fe5))
* **web:** introduce a compression middleware ([a406108](https://github.com/birdxs/magnetico/commit/a406108a9665858a68f05644838142cdde0996ad))
* **web:** set Content-Type header to text/html for HTML responses ([f6ee78a](https://github.com/birdxs/magnetico/commit/f6ee78a8e2ef940b3f0e3bee6d4845fa096c4592))
* **web:** update router to specify HTTP methods and add robots.txt handler ([206757e](https://github.com/birdxs/magnetico/commit/206757e9453e5d49c40d2bdaba214ec93e69e6b8))


### Bug Fixes

* added announce to torrent spec ([70a307a](https://github.com/birdxs/magnetico/commit/70a307a5ea079656c59370ee067912f2f985ee9c))
* **bencode:** impossible condition nil != nil ([c36c58b](https://github.com/birdxs/magnetico/commit/c36c58b8af0ec0c1f836bc1f2817927b8f70154e))
* **bencode:** return empty value instead of panic ([52e9999](https://github.com/birdxs/magnetico/commit/52e999914ad5115ad71d55e846796d8ec1bc22d3))
* can not download invalid utf8 name with BestName and BestPath ([#915](https://github.com/birdxs/magnetico/issues/915)) ([e6be81d](https://github.com/birdxs/magnetico/commit/e6be81dd57133daaf7e5624b85f7f50a1f44b53e))
* **ci:** do not run codecov on main ([9e596e8](https://github.com/birdxs/magnetico/commit/9e596e88c386c76e3a993358a235862ef7a8e6b6))
* **ci:** enable cache support ([a8d2a49](https://github.com/birdxs/magnetico/commit/a8d2a49764e603d3f3cda07303b346e6fd360254))
* **ci:** reintroduce the go workflow on PRs ([fd12437](https://github.com/birdxs/magnetico/commit/fd124373774b35bc04c257ccf5218030f4133066))
* **ci:** replace actions/delete-package-versions with dataaxiom/ghcr-cleaner-action ([8838565](https://github.com/birdxs/magnetico/commit/8838565c4bd197c0466b39a1ae38c3258a02ffde))
* **ci:** switch to hosted runners ([921a369](https://github.com/birdxs/magnetico/commit/921a3690ed4d9af7ae62168ecf5b6e8c7a964fa0))
* clear UPNP port mappings when client close ([#942](https://github.com/birdxs/magnetico/issues/942)) ([d0fa45d](https://github.com/birdxs/magnetico/commit/d0fa45dea2f4b081180745f8a1489570f4117978))
* **deps:** `go mod tidy` ([492b3b3](https://github.com/birdxs/magnetico/commit/492b3b3600cfe333b08762a9654d7144711fdf13))
* **deps:** drop a benchmark to unload a bunch of dependencies ([61c3239](https://github.com/birdxs/magnetico/commit/61c3239ff2c7a3714b769391408b4c68643c44b8))
* **deps:** replace gopkg.in/yaml.v3 with github.com/goccy/go-yaml ([3493828](https://github.com/birdxs/magnetico/commit/349382827e43b2d68cb30e542b043a77e6951675))
* **deps:** revert go-sqlite3 to v2.0.3+incompatible ([c4b1fc4](https://github.com/birdxs/magnetico/commit/c4b1fc453f594ce75799f1f4e439a197ee0386a9))
* **dht:** correct slice reinitialization issue in CompactNodeInfo Marshaler ([a72de2c](https://github.com/birdxs/magnetico/commit/a72de2c3c2a521f6365ea0645fb86dc2f9374bd8))
* **dht:** ignore nodes that have invalid ports ([819d2dd](https://github.com/birdxs/magnetico/commit/819d2dd4e65b73d8252a22fa3992d38c36aa8f9b))
* **dht:** increase chan size but do not drop idx results ([8300868](https://github.com/birdxs/magnetico/commit/830086829bfdcf24675ae25b93316f6ae36304df))
* **dht:** limit the number of nodes returned by dump ([1facb2b](https://github.com/birdxs/magnetico/commit/1facb2b416505a0106b5a26e61a0f728e652fe0d))
* **dht:** this method cannot run in a goroutine because msg is shared ([f1cb43a](https://github.com/birdxs/magnetico/commit/f1cb43a77b1c88bfddafc2f2b62354a37cc87c82))
* **docker:** cgo build ([cc4768f](https://github.com/birdxs/magnetico/commit/cc4768f818216de24b556760070efef10f2744ee))
* **gci:** file is not `gci`-ed with --skip-generated -s standard -s default ([b746785](https://github.com/birdxs/magnetico/commit/b746785568e1a40e348f78aff559ba87ca7bc840))
* **infohash:** gracefully handle bad hex strings without panicking ([ab2e677](https://github.com/birdxs/magnetico/commit/ab2e6772ac36de6e5b1c20758b4e59df773cff47))
* invalid Go toolchain version ([6a92690](https://github.com/birdxs/magnetico/commit/6a92690cb4f79355a679327ecbad4b55d9b7e2e0))
* label multicow build stage correctly ([f9d6146](https://github.com/birdxs/magnetico/commit/f9d61467478d6357afbfbbd0cfb986861c11f241))
* **linter:** bump golangci configuration format to the v2 syntax ([73e0b4b](https://github.com/birdxs/magnetico/commit/73e0b4b1c2cc82d82584b461927e9d81468c85d4))
* **linter:** starting from 1.22 go creates new variables for each iteration ([78962e8](https://github.com/birdxs/magnetico/commit/78962e8a9401ced3193146b564bbd12de011f0f0))
* **lint:** introduce rollback with error checking in sqlite ([13b38e1](https://github.com/birdxs/magnetico/commit/13b38e1404d4557ff74689113f8a1c87e679332f))
* **mainline:** add support for unmarshaling IPv6 addresses ([a5daa97](https://github.com/birdxs/magnetico/commit/a5daa974bfe38230931612d3edd594463d62d7d7))
* **mainline:** fallback to pseudo-random during token secret generation ([bb19d0a](https://github.com/birdxs/magnetico/commit/bb19d0a2168ad37ec8d7b913d055b7c3188780ef))
* **mainline:** Fix routingTable locking issue ([98e9f02](https://github.com/birdxs/magnetico/commit/98e9f02d6d7fa2c7aac7b9d4312840e527474b32))
* **mainline:** ipv6 compatibility for `UnmarshalCompactNodeInfos` ([8b5cfb4](https://github.com/birdxs/magnetico/commit/8b5cfb44e7b906eb29c884ab5a2ec99acb04c4ac))
* **mainline:** randomize nodeID ([793668c](https://github.com/birdxs/magnetico/commit/793668c7fa90fa81bffe189e57667ec021239951))
* **mainline:** Run initial index instantly  ([a4d66be](https://github.com/birdxs/magnetico/commit/a4d66bebb8a6c10953a561aeb71bb84845efcacf))
* **makefile:** fix the format target ([9c835b0](https://github.com/birdxs/magnetico/commit/9c835b0abf6e3ddb0bd360e051e3ca42ab016e24))
* **makefile:** missing tag during unit testing ([2b7ec58](https://github.com/birdxs/magnetico/commit/2b7ec58fbd77821fcc4c1077bd7624a6bba70fcb))
* **metadata:** avoid panic - return an error ([67946af](https://github.com/birdxs/magnetico/commit/67946af3a01220aae560294e3454eda93d547ec9))
* **metadata:** avoid panic - return nil ([e3676f8](https://github.com/birdxs/magnetico/commit/e3676f801bc6d37d94ae903a293e0c829a6fbf57))
* **metadata:** change the code logic to avoid a race condition ([d6b8f7e](https://github.com/birdxs/magnetico/commit/d6b8f7e7e73610e2c02a48f02449a4930a41a23b))
* **metadata:** delete on `len(peers) == 1` ([dfd2aa0](https://github.com/birdxs/magnetico/commit/dfd2aa08503dd3e8ef9afae6f6144808285167f5))
* **metadata:** err is nil here (nil pointer dereference) ([66abd60](https://github.com/birdxs/magnetico/commit/66abd604aadaa62b3913a4fae4254102b83cee45))
* **metadata:** fallback on math/rand when crypto/rand fails ([f7c7dee](https://github.com/birdxs/magnetico/commit/f7c7dee91c29301e28cfabc5ec72ee08de0535fe))
* **metadata:** ipv6 compatibility for `Leech` ([0c688e0](https://github.com/birdxs/magnetico/commit/0c688e07791c07bdc926711fcd874f7e378e94b2))
* **metadata:** leechers gets all used up ([a98fa14](https://github.com/birdxs/magnetico/commit/a98fa14fa62eedebd42a46ed9a5dc7cc287a4328))
* **metadata:** make V1Length avoid panic and return 0 ([586e548](https://github.com/birdxs/magnetico/commit/586e54891525744eee4322ae96274e6352b42b2d))
* **metadata:** report error when metadata size is zero ([e0fa28c](https://github.com/birdxs/magnetico/commit/e0fa28c5f682b67a71c762f78e48d9f1d109e564))
* **metadata:** restore the original login in onLeechError ([7ab675b](https://github.com/birdxs/magnetico/commit/7ab675bb249d7d0c11bef34ab844cbb8a6507614))
* **metainfo:** empty Info marshalling test ([d1b3b3a](https://github.com/birdxs/magnetico/commit/d1b3b3aa4dadecc84684446d370cebaab702d312))
* **metainfo:** return an error when the decoded length is wrong ([3f5f14d](https://github.com/birdxs/magnetico/commit/3f5f14d1c626e9b74b8df4ff2a5fb8cf4be7a4f9))
* **metainfo:** stdlib integration ([535dc08](https://github.com/birdxs/magnetico/commit/535dc08b6f81ccb070a2dfb056496d84e8a2cbbb))
* **oci:** add missing sbom generation and provenance support ([8baf52b](https://github.com/birdxs/magnetico/commit/8baf52baf58f6a7ea3779b1623adb4fd66b0e6f9))
* **oci:** add some recommended labels ([ff520d6](https://github.com/birdxs/magnetico/commit/ff520d661c0ea06188e2618780b44443530d627c))
* **oci:** add zeromq dependencies in oci image build ([4ec62bb](https://github.com/birdxs/magnetico/commit/4ec62bba9516543197c10b700486831ef02703ac))
* **oci:** avoid dev deps installation in the final container ([914ddd4](https://github.com/birdxs/magnetico/commit/914ddd4f7b756507490cdfb99dede3f93b074db0))
* **oci:** harden runtime image by switching to chainguard/static ([54a229b](https://github.com/birdxs/magnetico/commit/54a229b03b1d4d3a2cf1e476d3887e15db150bd8))
* **oci:** the 'as' keyword should match the case of the 'from' keyword ([bf557ed](https://github.com/birdxs/magnetico/commit/bf557ed8e6c159e62c035fabdcc4a6373ec453e4))
* **oci:** update dockerfile to use clang for building ([a368255](https://github.com/birdxs/magnetico/commit/a3682556d16e1d784492672862e3acd61fa637f7))
* **oom:** lower the default `indexer-max-neighbors` to 5000 peers ([132bf1b](https://github.com/birdxs/magnetico/commit/132bf1bbdb3b5fea22f5b1e923596263ad731237))
* **opflags:** detect invocation via magneticod or magneticow symlinks ([d1f7cf3](https://github.com/birdxs/magnetico/commit/d1f7cf3e04d2888df1e68d30467d3671cb0a1c10))
* **opflags:** exit gracefully if invoked with the help flag ([ef502d6](https://github.com/birdxs/magnetico/commit/ef502d6aea6127e2da0ddad6313c0404d6e96de5))
* **opflags:** restore the logic that sets both daemon and web to “on” if neither parameter is specified ([e130092](https://github.com/birdxs/magnetico/commit/e130092009f6a9dc6672aa4431960ffb7eb75553))
* **persistence:** change signature to match the interface ([df4e1ee](https://github.com/birdxs/magnetico/commit/df4e1eeac5053fdbc8e3920b2d033e0cbdd8a5c9))
* **persistence:** do not try to mess with the schema ([7619aaf](https://github.com/birdxs/magnetico/commit/7619aaf97ff4a43009cf0675093d81fc3f3ad805))
* **persistence:** handle parameters passed to postgres with zero values ([dbd4032](https://github.com/birdxs/magnetico/commit/dbd403245044e529de25f7fda6b03471fa05a29d))
* **persistence:** improve postgres and unify cockroach ([7f542d4](https://github.com/birdxs/magnetico/commit/7f542d455b11d097d27679b431bcfcb7cb49be49))
* **persistence:** redundant query getter ([7538623](https://github.com/birdxs/magnetico/commit/75386235f5b0596a556983c018b617519e755c1c))
* **persistence:** replace zeromq deps with the gopkg.in counterpart ([a75f859](https://github.com/birdxs/magnetico/commit/a75f859615c8014cbd99b5cf96b5e2146c524ab4))
* **persistence:** return an invalid value - avoid panics ([7e43e10](https://github.com/birdxs/magnetico/commit/7e43e105f2dfec60429efa9625a0f6f4a14c22df))
* **persistence:** rows might be nil if err != nil ([8f09f8e](https://github.com/birdxs/magnetico/commit/8f09f8eefe377af1ac68381d805bc73625da7251))
* **persistence:** rows might be nil if err != nil ([c61d863](https://github.com/birdxs/magnetico/commit/c61d86319e0eaaaeb17455c706394efa4d9df7e6))
* **persistence:** update the zeromq integration to use pebbe/zmq4 ([4af4ba3](https://github.com/birdxs/magnetico/commit/4af4ba35d3a3133b7d6930a0792b38a164ae5521))
* **persistence:** use tags fts5 ([c9b692d](https://github.com/birdxs/magnetico/commit/c9b692dfa33b272464a125295e4116b136b142f8))
* **persistence:** workaround for error with sqlite ≥ 3.34 ([f30db28](https://github.com/birdxs/magnetico/commit/f30db28e0d11b76fd591c9868415a808fe1bdb38))
* **readme:** remove lint badge [skip ci] ([8191f79](https://github.com/birdxs/magnetico/commit/8191f79db4ebbdc92b91fadb8cf4702a36f74ea2))
* remove go:build statement ([2c09c90](https://github.com/birdxs/magnetico/commit/2c09c90ff20e7a768d068a4063c6f50f9f9cd177))
* torrent file real time completed bytes ([ca5bd29](https://github.com/birdxs/magnetico/commit/ca5bd29a04d8a90224ac7a3c524354b9171a599c))
* **torrent:** InsecureSkipVerify should not be used in production code ([ed43794](https://github.com/birdxs/magnetico/commit/ed43794cc18986550acdc644db4c5d2096e7dbe6))
* **transport:** ipv6 compatibility for `Transport` ([09d7232](https://github.com/birdxs/magnetico/commit/09d7232223adac44ddd34f6e366f2ddf8dccc602))
* udp tracker panic ([8229ac4](https://github.com/birdxs/magnetico/commit/8229ac4b3f58fbd3b8d57c1f7ab2a71b4f764d32))
* upnp clear loop trap ([#946](https://github.com/birdxs/magnetico/issues/946)) ([f705f59](https://github.com/birdxs/magnetico/commit/f705f594bd5c0ab18642717e2db98c1767d6f03a))
* **util:** don't try to validate inet6 socks ([f9bfce9](https://github.com/birdxs/magnetico/commit/f9bfce92b1fe53ffa469818cbf074166875f9c4a))
* **web:** correct property name for discoveredOn in torrent data ([b6bcc68](https://github.com/birdxs/magnetico/commit/b6bcc6806af645edb9d7e62a9c7d4c20547e1961))
* **web:** don't use HTML entities when building URL (12c79539 fix-up) ([aff9ee5](https://github.com/birdxs/magnetico/commit/aff9ee566fdb638252b954287109c180b71979c7))
* **web:** drop the assets related to the readme endpoint ([a1884eb](https://github.com/birdxs/magnetico/commit/a1884eb8c15dcbf83c213164e107e122bdad8509))
* **web:** remove two debugging messages from the statistics page ([4d1097f](https://github.com/birdxs/magnetico/commit/4d1097ffca156d04f87bf4b1069e96a07fd5b66d))
* **web:** the rss feed should list the most common torrents ([4ebae27](https://github.com/birdxs/magnetico/commit/4ebae270c766662694d8afb8334cc3b14ed6a0aa))


### Performance Improvements

* **dht:** `rt.nodes` - avoid excessive allocations ([3ced3c6](https://github.com/birdxs/magnetico/commit/3ced3c66d4a8c5392c23982614f9120ed3f7de51))
* **dht:** adaptive crawling rate ([32b6db8](https://github.com/birdxs/magnetico/commit/32b6db833165d27673b18afd25976aaae3283c09))
* **dht:** add slice of neighbors in the routing table ([f115de1](https://github.com/birdxs/magnetico/commit/f115de1a7ea4973fd7a7fde73bf30213113b12ce))
* **dht:** discard old entries in the routing table if it gets too big ([1339624](https://github.com/birdxs/magnetico/commit/13396242fb1972a928b11d44c792bac659d26ac7))
* **dht:** on sample_infohash query received send a find_node query ([dc0e761](https://github.com/birdxs/magnetico/commit/dc0e76124284bf63a07bc6d14257534aadcc19b4))
* **dht:** prioritize `get_peers` and `find_node` queries ([565801a](https://github.com/birdxs/magnetico/commit/565801a86f9767a06dfd6e25437a5b9779512947))
* **dht:** use swiss tables for nodes routing ([88b33ea](https://github.com/birdxs/magnetico/commit/88b33ea8fcfcd5c7ac23101578031f3bb05d6c58))
* **magneticod:** raise the default value of parameters ([2bca306](https://github.com/birdxs/magnetico/commit/2bca3065dca1e250246dce98c5beb98c0941efbf))
* **mainline:** expand bep51 support - use goroutines ([18fafc7](https://github.com/birdxs/magnetico/commit/18fafc7e2f567da25a2a930c97aa3e593c8a488c))
* **metadata:** force mse - avoid throttling ([7c84ab4](https://github.com/birdxs/magnetico/commit/7c84ab45eea6a91f77472f330f703dd727ed4968))
* **metadata:** use a RW Mutex for incomingInfoHashesMx ([1ed13a1](https://github.com/birdxs/magnetico/commit/1ed13a1f70bef1db8a64d8155e42f28f38afe7a3))
* **persistence:** implement partitioning for files table in postgresql ([f4bf572](https://github.com/birdxs/magnetico/commit/f4bf572b2b78b421df16c851fc661d05c91bfd0c))
* **persistence:** improve the count method for torrents ([0e995d4](https://github.com/birdxs/magnetico/commit/0e995d4bd72b8aa361e9653ccf2f50472ad25441))
* **persistence:** move the temp_store in ram ([7da8980](https://github.com/birdxs/magnetico/commit/7da8980f7dc054cd3162220743fa67efd75c512f))
* **persistence:** remove postgres parameters inherited from the sqlite implementation ([e8ab03b](https://github.com/birdxs/magnetico/commit/e8ab03b302c3168fe220a433d789fd0e4692ae7e))


### Reverts

* Revert "Switch requestState to be a slice" ([8ccacbf](https://github.com/birdxs/magnetico/commit/8ccacbfd17154cedcb99a08438ef4175622ecdd7))
* Revert "fs/test.sh: Use go run instead of godo" ([7995958](https://github.com/birdxs/magnetico/commit/79959587cd907eed21526568388d7735b4777f13))
* Revert "Link to godocs.io for documentation" ([cd9a3a1](https://github.com/birdxs/magnetico/commit/cd9a3a14ad108efef3c450f5e7b4f7be9f2af9a5))
* Revert "Use a flat slice for pending request counts" ([8ddbf5a](https://github.com/birdxs/magnetico/commit/8ddbf5a852e5090c3060f32ec92113b1a62bf342))
* Revert "Remove old-style build tags" ([013634d](https://github.com/birdxs/magnetico/commit/013634d9f13a7152490bcb9ce3135f74435bc529))
* Revert "Fix stalls for responsive transfer tests" ([6bc2a2a](https://github.com/birdxs/magnetico/commit/6bc2a2a6ace24d5ea620a02acb920a224a0d57ae))
* Revert "Make requestStrategy 3 the default" ([a8787e6](https://github.com/birdxs/magnetico/commit/a8787e66323c0f5e9accb8c30f6858c80219a5a7))
* Revert "Quick fix for missing MetaInfo.Announce everywhere with trackers" ([a959bdd](https://github.com/birdxs/magnetico/commit/a959bdd0f823e6d46df984ebc7b19f9c9d9523c7))
* Revert "bencode: Trailing bytes on Unmarshal is an error" ([577ea21](https://github.com/birdxs/magnetico/commit/577ea21793e206adcc55d74789d72335c9f37e7e))


### Miscellaneous Chores

* **mainline:** stats should be tracked in a separate struct ([c4554d0](https://github.com/birdxs/magnetico/commit/c4554d0d9e28866bc5ba69ae9ff68c8dbe1c37ba))
* **persistence:** drop support for stdout ([75e5ed6](https://github.com/birdxs/magnetico/commit/75e5ed6cda114936b2573c88ee19e4599d944f55))


### Code Refactoring

* review the logic related to the operational flags ([0f02c84](https://github.com/birdxs/magnetico/commit/0f02c8446b2e3199e7cdfe13fa9bb3690b3e3bad))

## [2.3.0](https://github.com/tgragnato/magnetico/compare/v2.2.1...v2.3.0) (2025-06-28)


### Features

* **persistence:** allows postgres to find torrents by searching for file names ([c81b406](https://github.com/tgragnato/magnetico/commit/c81b40677a0ca73ed7865a4774c52e072d709269))


### Bug Fixes

* **oci:** add missing sbom generation and provenance support ([8baf52b](https://github.com/tgragnato/magnetico/commit/8baf52baf58f6a7ea3779b1623adb4fd66b0e6f9))


### Performance Improvements

* **persistence:** implement partitioning for files table in postgresql ([f4bf572](https://github.com/tgragnato/magnetico/commit/f4bf572b2b78b421df16c851fc661d05c91bfd0c))

## [2.2.1](https://github.com/tgragnato/magnetico/compare/v2.2.0...v2.2.1) (2025-05-04)


### Bug Fixes

* **deps:** replace gopkg.in/yaml.v3 with github.com/goccy/go-yaml ([3493828](https://github.com/tgragnato/magnetico/commit/349382827e43b2d68cb30e542b043a77e6951675))
* **linter:** bump golangci configuration format to the v2 syntax ([73e0b4b](https://github.com/tgragnato/magnetico/commit/73e0b4b1c2cc82d82584b461927e9d81468c85d4))
* **oci:** harden runtime image by switching to chainguard/static ([54a229b](https://github.com/tgragnato/magnetico/commit/54a229b03b1d4d3a2cf1e476d3887e15db150bd8))
* **opflags:** detect invocation via magneticod or magneticow symlinks ([d1f7cf3](https://github.com/tgragnato/magnetico/commit/d1f7cf3e04d2888df1e68d30467d3671cb0a1c10))
* **persistence:** update the zeromq integration to use pebbe/zmq4 ([4af4ba3](https://github.com/tgragnato/magnetico/commit/4af4ba35d3a3133b7d6930a0792b38a164ae5521))

## [2.2.0](https://github.com/tgragnato/magnetico/compare/v2.1.0...v2.2.0) (2025-02-25)


### Features

* **persistence:** add database import functionality ([6f0cfb1](https://github.com/tgragnato/magnetico/commit/6f0cfb1141c36b27e5c9c85cbfb990a5e8a478d7))
* **persistence:** implement database export functionality ([c804674](https://github.com/tgragnato/magnetico/commit/c80467425edd3a8da0e9f228e624ab1c38b16a26))
* **persistence:** implement export method for database interfaces ([7a705a6](https://github.com/tgragnato/magnetico/commit/7a705a69e08b3c9e968a68f8807533715ddbfae7))
* **stats:** add pyroscope profiling support ([5d261e1](https://github.com/tgragnato/magnetico/commit/5d261e12df1e29445a03e9bc5478729efef2900d))
* **web:** add redirect for non-root paths and handle invalid methods ([3604006](https://github.com/tgragnato/magnetico/commit/360400601ab494a68accb06e455ceac2db060554))
* **web:** add timeout configuration for web interface and apis ([2255959](https://github.com/tgragnato/magnetico/commit/225595982cdf094762aabe99d809ca76c1104fe5))
* **web:** introduce a compression middleware ([a406108](https://github.com/tgragnato/magnetico/commit/a406108a9665858a68f05644838142cdde0996ad))
* **web:** set Content-Type header to text/html for HTML responses ([f6ee78a](https://github.com/tgragnato/magnetico/commit/f6ee78a8e2ef940b3f0e3bee6d4845fa096c4592))
* **web:** update router to specify HTTP methods and add robots.txt handler ([206757e](https://github.com/tgragnato/magnetico/commit/206757e9453e5d49c40d2bdaba214ec93e69e6b8))


### Bug Fixes

* **oci:** update dockerfile to use clang for building ([a368255](https://github.com/tgragnato/magnetico/commit/a3682556d16e1d784492672862e3acd61fa637f7))


### Performance Improvements

* **dht:** use swiss tables for nodes routing ([88b33ea](https://github.com/tgragnato/magnetico/commit/88b33ea8fcfcd5c7ac23101578031f3bb05d6c58))

## [2.1.0](https://github.com/tgragnato/magnetico/compare/v2.0.0...v2.1.0) (2025-01-04)


### Features

* add api endpoint to get total count of torrents based on query keyword ([bd5c138](https://github.com/tgragnato/magnetico/commit/bd5c138bba29c9e1b7430fc1fa82f4b2320c91e2))
* **web:** add new parameters with different semantics to the `torrentstotal` api ([fc60049](https://github.com/tgragnato/magnetico/commit/fc60049ad9f4ed417bdb2e186ddb22a270d98127))


### Bug Fixes

* **web:** correct property name for discoveredOn in torrent data ([b6bcc68](https://github.com/tgragnato/magnetico/commit/b6bcc6806af645edb9d7e62a9c7d4c20547e1961))
* **web:** don't use HTML entities when building URL (12c79539 fix-up) ([aff9ee5](https://github.com/tgragnato/magnetico/commit/aff9ee566fdb638252b954287109c180b71979c7))
* **web:** remove two debugging messages from the statistics page ([4d1097f](https://github.com/tgragnato/magnetico/commit/4d1097ffca156d04f87bf4b1069e96a07fd5b66d))


### Performance Improvements

* **persistence:** improve the count method for torrents ([0e995d4](https://github.com/tgragnato/magnetico/commit/0e995d4bd72b8aa361e9653ccf2f50472ad25441))

## [2.0.0](https://github.com/tgragnato/magnetico/compare/v1.62.0...v2.0.0) (2024-11-30)


### ⚠ BREAKING CHANGES

* review the logic related to the operational flags
* introduce the ability to use a configuration file
* allow user supplied ports for bootstrap nodes

### Features

* allow user supplied ports for bootstrap nodes ([774ed20](https://github.com/tgragnato/magnetico/commit/774ed206dd7c473a4004083b697f1e4c011b4f88))
* introduce the ability to use a configuration file ([6eb27c2](https://github.com/tgragnato/magnetico/commit/6eb27c2a17f8ff3db92b2e40cc413a4d779c63ea))
* **opflags:** add a flag for the deadline of leeches ([9709b18](https://github.com/tgragnato/magnetico/commit/9709b1863381fe0bf440cd4bb16eda99bf40db01))
* **persistence:** add rabbitmq amqp basic support ([24925ba](https://github.com/tgragnato/magnetico/commit/24925ba2f5896fffcef183067fa709733b998457))
* **persistence:** add support for the bitmagnet import api ([0a4579d](https://github.com/tgragnato/magnetico/commit/0a4579d496ce27f06e17c4d276d28bf8ddcf74f8))
* **persistence:** perform pattern matching without case sensitivity ([b27c8b1](https://github.com/tgragnato/magnetico/commit/b27c8b130aef60a134ef99d033d6e6222ff26dbf))
* **web:** add count parameter to rss feed ([8e7d2cf](https://github.com/tgragnato/magnetico/commit/8e7d2cfdb277aaff814df99e46b13859be72ac65))


### Bug Fixes

* **gci:** file is not `gci`-ed with --skip-generated -s standard -s default ([b746785](https://github.com/tgragnato/magnetico/commit/b746785568e1a40e348f78aff559ba87ca7bc840))
* **metadata:** avoid panic - return nil ([e3676f8](https://github.com/tgragnato/magnetico/commit/e3676f801bc6d37d94ae903a293e0c829a6fbf57))
* **metadata:** make V1Length avoid panic and return 0 ([586e548](https://github.com/tgragnato/magnetico/commit/586e54891525744eee4322ae96274e6352b42b2d))
* **metainfo:** return an error when the decoded length is wrong ([3f5f14d](https://github.com/tgragnato/magnetico/commit/3f5f14d1c626e9b74b8df4ff2a5fb8cf4be7a4f9))
* **opflags:** exit gracefully if invoked with the help flag ([ef502d6](https://github.com/tgragnato/magnetico/commit/ef502d6aea6127e2da0ddad6313c0404d6e96de5))
* **opflags:** restore the logic that sets both daemon and web to “on” if neither parameter is specified ([e130092](https://github.com/tgragnato/magnetico/commit/e130092009f6a9dc6672aa4431960ffb7eb75553))
* **persistence:** handle parameters passed to postgres with zero values ([dbd4032](https://github.com/tgragnato/magnetico/commit/dbd403245044e529de25f7fda6b03471fa05a29d))
* **web:** the rss feed should list the most common torrents ([4ebae27](https://github.com/tgragnato/magnetico/commit/4ebae270c766662694d8afb8334cc3b14ed6a0aa))


### Performance Improvements

* **persistence:** remove postgres parameters inherited from the sqlite implementation ([e8ab03b](https://github.com/tgragnato/magnetico/commit/e8ab03b302c3168fe220a433d789fd0e4692ae7e))


### Code Refactoring

* review the logic related to the operational flags ([0f02c84](https://github.com/tgragnato/magnetico/commit/0f02c8446b2e3199e7cdfe13fa9bb3690b3e3bad))

## [1.62.0](https://github.com/tgragnato/magnetico/compare/v1.61.2...v1.62.0) (2024-09-23)


### Features

* **dht:** implement NewSampleInfohashesResponse and onSampleInfohashesQuery ([6d69021](https://github.com/tgragnato/magnetico/commit/6d69021c26526a04855e7d35c0dfcc138172b02e))
* **dht:** introduce support for the ipv6 krpc protocol ([66fc7b0](https://github.com/tgragnato/magnetico/commit/66fc7b098eb3e09021df84dd0dc0e680f4554f73))
* **metainfo:** support for serializing v2 torrent file ([a8c2460](https://github.com/tgragnato/magnetico/commit/a8c2460727c2aeb01b16783342651d3606c10794))
* **stats:** add prometheus exporter for application metrics ([fc12657](https://github.com/tgragnato/magnetico/commit/fc126578bce118aba0ee1b19565984973a85ec28))


### Bug Fixes

* **bencode:** return empty value instead of panic ([52e9999](https://github.com/tgragnato/magnetico/commit/52e999914ad5115ad71d55e846796d8ec1bc22d3))
* **metadata:** avoid panic - return an error ([67946af](https://github.com/tgragnato/magnetico/commit/67946af3a01220aae560294e3454eda93d547ec9))
* **metadata:** report error when metadata size is zero ([e0fa28c](https://github.com/tgragnato/magnetico/commit/e0fa28c5f682b67a71c762f78e48d9f1d109e564))
* **metainfo:** empty Info marshalling test ([d1b3b3a](https://github.com/tgragnato/magnetico/commit/d1b3b3aa4dadecc84684446d370cebaab702d312))
* **metainfo:** stdlib integration ([535dc08](https://github.com/tgragnato/magnetico/commit/535dc08b6f81ccb070a2dfb056496d84e8a2cbbb))
* **persistence:** change signature to match the interface ([df4e1ee](https://github.com/tgragnato/magnetico/commit/df4e1eeac5053fdbc8e3920b2d033e0cbdd8a5c9))
* **persistence:** workaround for error with sqlite ≥ 3.34 ([f30db28](https://github.com/tgragnato/magnetico/commit/f30db28e0d11b76fd591c9868415a808fe1bdb38))


### Performance Improvements

* **metadata:** force mse - avoid throttling ([7c84ab4](https://github.com/tgragnato/magnetico/commit/7c84ab45eea6a91f77472f330f703dd727ed4968))

## [1.61.2](https://github.com/tgragnato/magnetico/compare/v1.61.1...v1.61.2) (2024-09-03)


### Bug Fixes

* **oci:** add some recommended labels ([ff520d6](https://github.com/tgragnato/magnetico/commit/ff520d661c0ea06188e2618780b44443530d627c))


### Performance Improvements

* **dht:** adaptive crawling rate ([32b6db8](https://github.com/tgragnato/magnetico/commit/32b6db833165d27673b18afd25976aaae3283c09))

## [1.61.1](https://github.com/tgragnato/magnetico/compare/v1.61.0...v1.61.1) (2024-09-01)


### Bug Fixes

* **dht:** this method cannot run in a goroutine because msg is shared ([f1cb43a](https://github.com/tgragnato/magnetico/commit/f1cb43a77b1c88bfddafc2f2b62354a37cc87c82))

## [1.61.0](https://github.com/tgragnato/magnetico/compare/v1.60.1...v1.61.0) (2024-09-01)


### Features

* **dht:** implement support for additional mainline methods ([db977b7](https://github.com/tgragnato/magnetico/commit/db977b7dcfb056e7f20604283f7a2a4b3c4ff381))
* flush metrics every minute ([de6001b](https://github.com/tgragnato/magnetico/commit/de6001b6fdaaa46f6dab8476813c7439bb3c59a6))
* **metadata:** add support for message stream encryption ([783dca8](https://github.com/tgragnato/magnetico/commit/783dca89fb4ff56ccb6b10f6a4e0e2df3d8acf03))
* **metadata:** add support for Multipath TCP ([e81f3b1](https://github.com/tgragnato/magnetico/commit/e81f3b1e4ccdfe0926de070b222a2629859ed7ba))
* **persistence:** implement a ZeroMQ interface ([a4654c2](https://github.com/tgragnato/magnetico/commit/a4654c2aeafc29e4aae2af3fb9696caebefce172))
* **persistence:** support both cgo and non-cgo builds ([96ee524](https://github.com/tgragnato/magnetico/commit/96ee524fe213076f02bfb42d35604e90c394cdef))
* **stats:** add a package for logging metrics ([c96820b](https://github.com/tgragnato/magnetico/commit/c96820b09179558ba2bfca34d3f879a7571a27a6))


### Bug Fixes

* **bencode:** impossible condition nil != nil ([c36c58b](https://github.com/tgragnato/magnetico/commit/c36c58b8af0ec0c1f836bc1f2817927b8f70154e))
* **dht:** correct slice reinitialization issue in CompactNodeInfo Marshaler ([a72de2c](https://github.com/tgragnato/magnetico/commit/a72de2c3c2a521f6365ea0645fb86dc2f9374bd8))
* **dht:** ignore nodes that have invalid ports ([819d2dd](https://github.com/tgragnato/magnetico/commit/819d2dd4e65b73d8252a22fa3992d38c36aa8f9b))
* **dht:** increase chan size but do not drop idx results ([8300868](https://github.com/tgragnato/magnetico/commit/830086829bfdcf24675ae25b93316f6ae36304df))
* **dht:** limit the number of nodes returned by dump ([1facb2b](https://github.com/tgragnato/magnetico/commit/1facb2b416505a0106b5a26e61a0f728e652fe0d))
* **infohash:** gracefully handle bad hex strings without panicking ([ab2e677](https://github.com/tgragnato/magnetico/commit/ab2e6772ac36de6e5b1c20758b4e59df773cff47))
* **metadata:** fallback on math/rand when crypto/rand fails ([f7c7dee](https://github.com/tgragnato/magnetico/commit/f7c7dee91c29301e28cfabc5ec72ee08de0535fe))
* **oci:** add zeromq dependencies in oci image build ([4ec62bb](https://github.com/tgragnato/magnetico/commit/4ec62bba9516543197c10b700486831ef02703ac))
* **oci:** avoid dev deps installation in the final container ([914ddd4](https://github.com/tgragnato/magnetico/commit/914ddd4f7b756507490cdfb99dede3f93b074db0))
* **oci:** the 'as' keyword should match the case of the 'from' keyword ([bf557ed](https://github.com/tgragnato/magnetico/commit/bf557ed8e6c159e62c035fabdcc4a6373ec453e4))
* **oom:** lower the default `indexer-max-neighbors` to 5000 peers ([132bf1b](https://github.com/tgragnato/magnetico/commit/132bf1bbdb3b5fea22f5b1e923596263ad731237))
* **persistence:** replace zeromq deps with the gopkg.in counterpart ([a75f859](https://github.com/tgragnato/magnetico/commit/a75f859615c8014cbd99b5cf96b5e2146c524ab4))
* **persistence:** return an invalid value - avoid panics ([7e43e10](https://github.com/tgragnato/magnetico/commit/7e43e105f2dfec60429efa9625a0f6f4a14c22df))
* **persistence:** rows might be nil if err != nil ([8f09f8e](https://github.com/tgragnato/magnetico/commit/8f09f8eefe377af1ac68381d805bc73625da7251))
* **persistence:** rows might be nil if err != nil ([c61d863](https://github.com/tgragnato/magnetico/commit/c61d86319e0eaaaeb17455c706394efa4d9df7e6))
* remove go:build statement ([2c09c90](https://github.com/tgragnato/magnetico/commit/2c09c90ff20e7a768d068a4063c6f50f9f9cd177))


### Performance Improvements

* **dht:** `rt.nodes` - avoid excessive allocations ([3ced3c6](https://github.com/tgragnato/magnetico/commit/3ced3c66d4a8c5392c23982614f9120ed3f7de51))
* **dht:** add slice of neighbors in the routing table ([f115de1](https://github.com/tgragnato/magnetico/commit/f115de1a7ea4973fd7a7fde73bf30213113b12ce))
* **dht:** discard old entries in the routing table if it gets too big ([1339624](https://github.com/tgragnato/magnetico/commit/13396242fb1972a928b11d44c792bac659d26ac7))
* **dht:** on sample_infohash query received send a find_node query ([dc0e761](https://github.com/tgragnato/magnetico/commit/dc0e76124284bf63a07bc6d14257534aadcc19b4))
* **dht:** prioritize `get_peers` and `find_node` queries ([565801a](https://github.com/tgragnato/magnetico/commit/565801a86f9767a06dfd6e25437a5b9779512947))

## [1.60.1](https://github.com/tgragnato/magnetico/compare/v1.60.0...v1.60.1) (2024-08-14)


### Bug Fixes

* **deps:** drop a benchmark to unload a bunch of dependencies ([61c3239](https://github.com/tgragnato/magnetico/commit/61c3239ff2c7a3714b769391408b4c68643c44b8))
* **web:** drop the assets related to the readme endpoint ([a1884eb](https://github.com/tgragnato/magnetico/commit/a1884eb8c15dcbf83c213164e107e122bdad8509))

## [1.60.0](https://github.com/tgragnato/magnetico/compare/v1.59.0...v1.60.0) (2024-08-13)


### Features

* add arm64 to multi-platform container builds ([4a09971](https://github.com/tgragnato/magnetico/commit/4a09971b9f9ecd26c7dc3f40c5290b0f6a6138c3))
* **ci:** publish multi-platform executables in releases ([89f7f02](https://github.com/tgragnato/magnetico/commit/89f7f020b6ccb20f80b54127d41c5004d542e5b1))


### Bug Fixes

* **ci:** enable cache support ([a8d2a49](https://github.com/tgragnato/magnetico/commit/a8d2a49764e603d3f3cda07303b346e6fd360254))
* **ci:** replace actions/delete-package-versions with dataaxiom/ghcr-cleaner-action ([8838565](https://github.com/tgragnato/magnetico/commit/8838565c4bd197c0466b39a1ae38c3258a02ffde))

## [1.59.0](https://github.com/tgragnato/magnetico/compare/v1.58.3...v1.59.0) (2024-08-13)


### Features

* add validation for filter-nodes-cidrs during parsing ([50e7717](https://github.com/tgragnato/magnetico/commit/50e77170a178e0c588c16cc3f19368896e06100b))
* **dht:** crawl only specified ip ranges ([acb1913](https://github.com/tgragnato/magnetico/commit/acb19137b5776343b8fa087615ee95ab4436eb70))


### Bug Fixes

* invalid Go toolchain version ([6a92690](https://github.com/tgragnato/magnetico/commit/6a92690cb4f79355a679327ecbad4b55d9b7e2e0))

