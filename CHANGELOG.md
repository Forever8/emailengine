# Changelog

## [2.38.0](https://github.com/postalsys/emailengine/compare/v2.37.7...v2.38.0) (2023-10-26)


### Features

* **oauth:** Allow to disable base OAuth2 scopes like SMTP.Send ([ef89d83](https://github.com/postalsys/emailengine/commit/ef89d83643b9a7c6d03aba04e75afcbcf0b611e9))
* **openai:** Allow to set custom models using the API (not in UI) ([858f48b](https://github.com/postalsys/emailengine/commit/858f48b8a69c850e8d491fc6d585243ae1c183ac))
* **openai:** Allow to specify custom API url for OpenAI API requests ([047647d](https://github.com/postalsys/emailengine/commit/047647df95c17f5cfbc11647eedd560e3659931e))
* **tls:** Allow to ignore IMAP/SMTP TLS certificate errors by default using the ignoreMailCertErrors setting ([cba8ffe](https://github.com/postalsys/emailengine/commit/cba8ffeca489321e3c9736039a325c8acfb05de2))


### Bug Fixes

* **special-use-flags:** Added support for user-specified Archive special use tag ([a107f23](https://github.com/postalsys/emailengine/commit/a107f233d9f25800c08dd3e371b7cd6c95fe1a1b))
* **throttling:** Retry throttled FETCH commands a few times before giving up ([c3d259a](https://github.com/postalsys/emailengine/commit/c3d259a0bc94cd3b84ffd6e77b77d1bc098ff64c))

## [2.37.7](https://github.com/postalsys/emailengine/compare/v2.37.6...v2.37.7) (2023-10-20)


### Bug Fixes

* **chat:** use topic instead of question for the filtering embedding ([3acebc3](https://github.com/postalsys/emailengine/commit/3acebc37dd5e5c0d25dab386354f1ec1bf78d244))
* **initialization:** Start all IMAP worker threads before assigning accounts ([9b4c3fc](https://github.com/postalsys/emailengine/commit/9b4c3fc48b00a3bcfeade592cc36b8144038dad8))
* **stats:** added missing counters for messageNew/messageDeleted ([3f9f4cd](https://github.com/postalsys/emailengine/commit/3f9f4cda6aa1896f7c30b786ab7909ea274fcb69))

## [2.37.6](https://github.com/postalsys/emailengine/compare/v2.37.5...v2.37.6) (2023-10-17)


### Bug Fixes

* **about:** Added a dedicated page for license and legal information ([077b38f](https://github.com/postalsys/emailengine/commit/077b38f4edfe711109fab809327adcaa55204b40))
* **accountCounters:** added counters object that contains cumulative counter of all account specific triggered events ([67613a3](https://github.com/postalsys/emailengine/commit/67613a3bb5e69dc06304a6a5441b997e52e7b5f1))
* **documentstore:** do not report missing email as an error ([58130c7](https://github.com/postalsys/emailengine/commit/58130c786b21fcb75ce48e557c5b8f19edbb7581))
* **license:** added a section to the license about source code usage ([a923d3b](https://github.com/postalsys/emailengine/commit/a923d3bba28bf3831aa79face17c75ad65ace002))

## [2.37.5](https://github.com/postalsys/emailengine/compare/v2.37.4...v2.37.5) (2023-10-11)


### Bug Fixes

* **chat:** Fixed chat feature support for older Redis versions ([86538ba](https://github.com/postalsys/emailengine/commit/86538baff7037598788e38b68495f4d3958d52bc))
* **default_conf:** Ensure default config values for notifyText, notifyTextSize, and enableApiProxy ([b7b4d9c](https://github.com/postalsys/emailengine/commit/b7b4d9c150ffabd533e5015b2e4aee4f26160b30))
* **license:** allow selecting license key from a file instead of copying ([d813e35](https://github.com/postalsys/emailengine/commit/d813e356a20879c7e9c69db9f8e21e5648be2a6d))

## [2.37.4](https://github.com/postalsys/emailengine/compare/v2.37.3...v2.37.4) (2023-10-05)


### Bug Fixes

* **docker:** fixed docker tags, added missing v prefix to version tags ([481bf5c](https://github.com/postalsys/emailengine/commit/481bf5c6e80b6cb48a32f460dd65ee887bc79847))

## [2.37.3](https://github.com/postalsys/emailengine/compare/v2.37.2...v2.37.3) (2023-10-05)


### Bug Fixes

* **docker:** fixed docker tagged release process ([f23cde0](https://github.com/postalsys/emailengine/commit/f23cde0e851fc3e43893383d65929dc3f03b2991))

## [2.37.2](https://github.com/postalsys/emailengine/compare/v2.37.1...v2.37.2) (2023-10-03)


### Bug Fixes

* **chat:** Bumped dependency to better parse output from OpenAI API ([0250da8](https://github.com/postalsys/emailengine/commit/0250da8c37b1ced730dc9e42a611e1d6bdc0a582))

## [2.37.1](https://github.com/postalsys/emailengine/compare/v2.37.0...v2.37.1) (2023-10-02)


### Bug Fixes

* **chat:** Added 'try it' button to 'chat with emails' config page ([0f23c39](https://github.com/postalsys/emailengine/commit/0f23c390887b6d554b2ed90a437c30f2c6530aac))
* **chat:** Improved 'chat with emails' response quality by sorting and filtering embeddings vectors ([de429d6](https://github.com/postalsys/emailengine/commit/de429d6f8f1cffdbce0e48dce4f716cdf83f93bf))

## [2.37.0](https://github.com/postalsys/emailengine/compare/v2.36.1...v2.37.0) (2023-09-29)


### Features

* **secrets:** removed deprecated vault support ([8ab9d60](https://github.com/postalsys/emailengine/commit/8ab9d60df58b5d258dcf459a1928f285b02eea62))


### Bug Fixes

* **chat:** Use separate settings page for 'chat with emails' feature ([c66e3ba](https://github.com/postalsys/emailengine/commit/c66e3ba8234390ccc5cf800cee29f8e4ab0b56d2))
* **deploy:** Build packages with Node 20 ([a394cf2](https://github.com/postalsys/emailengine/commit/a394cf2d487ba95a1906b964a630d524cf57f16c))
* **package-lock:** Do not delete package lock. Use 'npm ci' to install dependencies ([752be23](https://github.com/postalsys/emailengine/commit/752be230bf510c68c1551e0f852b47a7d1f1dedb))

## [2.36.1](https://github.com/postalsys/emailengine/compare/v2.36.0...v2.36.1) (2023-09-20)


### Bug Fixes

* **deploy:** keep package-lock.json ([ec311e3](https://github.com/postalsys/emailengine/commit/ec311e34834266d6a1db382dc044a13828a1eca4))

## [2.36.0](https://github.com/postalsys/emailengine/compare/v2.35.0...v2.36.0) (2023-09-20)


### Features

* **ai:** Allow using embeddings generation without prompting ([b59e702](https://github.com/postalsys/emailengine/commit/b59e702b31a869e810178518b9549871b7988b19))


### Bug Fixes

* **ai:** Added support for gpt-3.5-turbo-instruct ([bf75c5a](https://github.com/postalsys/emailengine/commit/bf75c5ab4077ffe5e0b4a92e009d4ee6500c50b8))
* **ai:** Do not store generated embeddings in the document store ([9638480](https://github.com/postalsys/emailengine/commit/9638480662581ed09bf7fa0ebecbb64461224413))
* **deploy:** Added tests runner ([b382569](https://github.com/postalsys/emailengine/commit/b382569604b74f312ab7fadafdcba65d76f0c1ec))
* **deploy:** Automated release management ([8e2bd88](https://github.com/postalsys/emailengine/commit/8e2bd88d305a8502102986528b346c96f35f4c06))
