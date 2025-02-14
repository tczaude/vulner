## [0.6.1](https://github.com/mrl5/vulner/compare/v0.6.0...v0.6.1) (2022-06-17)


### Bug Fixes

* **cli:** treat API key as a secret ([0b08d3e](https://github.com/mrl5/vulner/commit/0b08d3ed19f97992c883ead8d532cd083d861d99))



# [0.6.0](https://github.com/mrl5/vulner/compare/v0.5.0...v0.6.0) (2022-04-12)


### Bug Fixes

* cargo audit fix - drop chrono dependency [[#47](https://github.com/mrl5/vulner/issues/47)][[#48](https://github.com/mrl5/vulner/issues/48)] ([2da3ced](https://github.com/mrl5/vulner/commit/2da3cedd3c41e6bd700c0e0fddc50d09f639a197))
* **scan:** append package report file instead of truncate ([997c582](https://github.com/mrl5/vulner/commit/997c582dc48891c70d663ab6419b1da5b09e8cdf))


### Features

* **scan:** package name as report filename ([3f9fa67](https://github.com/mrl5/vulner/commit/3f9fa670d55881308fedc1d6e724c45566c9091e))


### Performance Improvements

* **cpe-tag:** avoid compiling the same regex in a loop ([e08f29e](https://github.com/mrl5/vulner/commit/e08f29e27db955a9de6288b2c5fa5c7f912f32b9))
* **scan:** allocate 40.8% less memory for cpe feed ([7ab77cf](https://github.com/mrl5/vulner/commit/7ab77cfa7fd18b7a386b500e4134d7cb71736985))



# [0.5.0](https://github.com/mrl5/vulner/compare/v0.4.0...v0.5.0) (2022-03-18)


### Bug Fixes

* **scan:** chmod 700 for scan results directory ([9281be3](https://github.com/mrl5/vulner/commit/9281be32f6ddfda0d209744d7a81c44ec673d7a5))


### Features

* **cli:** default out dir in local config ([f014ca7](https://github.com/mrl5/vulner/commit/f014ca742e89d9c5fa3bee54f91487d45c68b83c))
* **cli:** info as default log level ([9a5d613](https://github.com/mrl5/vulner/commit/9a5d61313b780bdc176866f17f71276d79815a32))
* **cli:** local config ([f7e3c68](https://github.com/mrl5/vulner/commit/f7e3c6801baa22d5cd3c16fb0e21190df0f35d6a))
* **cli:** support usage of NVD API key [[#31](https://github.com/mrl5/vulner/issues/31)] ([2168fc9](https://github.com/mrl5/vulner/commit/2168fc9a4fdf6b749b76df72ef9aeb8fdb8a7fc2))
* **scan:** support recursive scanning of funtoo meta-repo [[#29](https://github.com/mrl5/vulner/issues/29)] ([4ee8a5e](https://github.com/mrl5/vulner/commit/4ee8a5e2d9a8af2a1550fa9be52c631e1babf0cf))
* **scan:** support scanning the portage tree/kits of ebuilds [[#29](https://github.com/mrl5/vulner/issues/29)] ([338cbf0](https://github.com/mrl5/vulner/commit/338cbf0555882d46d6385a514017d546c544f743))



# [0.4.0](https://github.com/mrl5/vulner/compare/v0.3.1...v0.4.0) (2022-02-28)


### Features

* **cli:** kev - new command for printing known exploited vulnerabilities ([96bc9a3](https://github.com/mrl5/vulner/commit/96bc9a3766e97838c1e29d7214672b422f0a1493))
* **cli:** recognize known exploited CVEs ([c452ad9](https://github.com/mrl5/vulner/commit/c452ad947678604051d41f5732256ad70cac6641))



## [0.3.1](https://github.com/mrl5/vulner/compare/v0.3.0...v0.3.1) (2022-02-26)


### Bug Fixes

* adapter for apache http server ([e28c04a](https://github.com/mrl5/vulner/commit/e28c04ac1b08ccd6e2c89e692e421ba97dcaa970))



# [0.3.0](https://github.com/mrl5/vulner/compare/v0.2.0...v0.3.0) (2022-02-22)


### Features

* **cli:** allow defining pkg dir for scan [[#20](https://github.com/mrl5/vulner/issues/20)] ([057eab8](https://github.com/mrl5/vulner/commit/057eab85892d8570fbc06bfda71b3265de9045c9))



# [0.2.0](https://github.com/mrl5/vulner/compare/v0.1.0...v0.2.0) (2022-02-14)


### Bug Fixes

* **cli:** dont stop but log on http error ([b9494f5](https://github.com/mrl5/vulner/commit/b9494f506163997d719139ec03e887350f2f3f0c))
* **cpe-tag:** more verbose error when cpe match feed not found ([52f4061](https://github.com/mrl5/vulner/commit/52f4061d2e16dc2ea03db40905ce6e060876af5b))
* **os-adapter:** gentoo flavor is gentoo ([0e42c43](https://github.com/mrl5/vulner/commit/0e42c439e632a44ba6c326538159a8ae1254a7ad))


### Features

* **cli:** richer scan reports ([23799cc](https://github.com/mrl5/vulner/commit/23799ccad50e578abbe7cf2850c756a3c913b857))
* **cli:** summary flag for cve command ([890f588](https://github.com/mrl5/vulner/commit/890f5887aec4290224347a3a2f7d6f9025630a91))
* **os-adapter:** support gentoo linux ([3fcfce8](https://github.com/mrl5/vulner/commit/3fcfce81f89f52e5cd415917aa1fb42bc953788e))



# 0.1.0 (2022-01-30)


### Features

* **cli:** allow piping (input from stdin) ([790c5f6](https://github.com/mrl5/vulner/commit/790c5f607ecf934474a6898d3f69f658b4838ecf))
* **cli:** init CLI ([78b0d8d](https://github.com/mrl5/vulner/commit/78b0d8d7790073080eb10616dcbdc81b23e4d07e))
* cpe - new command for returning valid and existing CPEs ([bac30f5](https://github.com/mrl5/vulner/commit/bac30f5da64479ac25b1007402fe05720d9675f8))
* cve - new command for listing CVEs for given CPEs ([5b6ca09](https://github.com/mrl5/vulner/commit/5b6ca095fc1de36163d3ba36bd8f929a8144718c))
* **lib:** reuse python lib for grep patterns ([2dfcfcf](https://github.com/mrl5/vulner/commit/2dfcfcf703a1fc87eb3aca32b65281f486240181))
* scan - new command for CVE scanning ([5a96512](https://github.com/mrl5/vulner/commit/5a9651281da9cffad2432fc9d9f4164bf417f799))
* sync - new command for fetching NVD CPE match feed ([55e053d](https://github.com/mrl5/vulner/commit/55e053d129738293de7bb5714ead197d28330759))


### Performance Improvements

* **cpe:** deserialize from string only once ([47fe076](https://github.com/mrl5/vulner/commit/47fe0760a55cfc28b1804cd050455cee98c7cdcb))



