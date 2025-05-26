# Changelog

## [0.1.0](https://github.com/dbirks/claude-code-proxy/compare/v0.0.1...v0.1.0) (2025-05-26)


### Features

* Add a main() ([131346d](https://github.com/dbirks/claude-code-proxy/commit/131346de63e9914e716f93c65fb78190ef228de2))
* add provider preference and update model mapping. Introduce PREFERRED_PROVIDER env var (default: google). Update default BIG/SMALL models to Gemini latest. Refactor model mapping logic to respect provider preference. Add .env.example and update README. ([b64350d](https://github.com/dbirks/claude-code-proxy/commit/b64350df69206a5b8b998e64090db222364e726a))


### Bug Fixes

* Get the module and project.script working ([747dee7](https://github.com/dbirks/claude-code-proxy/commit/747dee7f44b988f4d3ded098ca939ef136f0767c))


### Documentation

* correct setup instructions to use uv ([3185e9f](https://github.com/dbirks/claude-code-proxy/commit/3185e9f6a7240c76806e9d7c96b2d14de0df9321))
* restore correct uv setup instructions ([f3282ca](https://github.com/dbirks/claude-code-proxy/commit/f3282ca21d72fbe9c0ae77bac48eb51d87d9b9d0))
* update README title and intro to be provider-neutral ([15d849c](https://github.com/dbirks/claude-code-proxy/commit/15d849cc0303a6dc66243df10eeef110bb961ae4))
* update README to reflect Gemini default and clarify config ([b5ff296](https://github.com/dbirks/claude-code-proxy/commit/b5ff29669fa331d68fb139b9c85ca36975fa1961))


### Miscellaneous Chores

* Configure Renovate ([#1](https://github.com/dbirks/claude-code-proxy/issues/1)) ([e9ed4ed](https://github.com/dbirks/claude-code-proxy/commit/e9ed4edecbccd130b9b1d6e61faf8070d0d35362))
* **deps:** update python to v3.13 ([#2](https://github.com/dbirks/claude-code-proxy/issues/2)) ([9b66511](https://github.com/dbirks/claude-code-proxy/commit/9b665111674ff74840e97f6537bff0fc8559444c))


### Code Refactoring

* set default provider to openai and update default models to gpt-4.1/mini ([e9c8cf8](https://github.com/dbirks/claude-code-proxy/commit/e9c8cf8de6e8f11cf54dd677634e9796e040f2fd))
* update default models to gemini 2.5/2.0 and remove 1.5 refs ([e07c97b](https://github.com/dbirks/claude-code-proxy/commit/e07c97b7a2cbe36d64b7fc10c763e26d7f628caf))


### Build System

* Start adding build-system ([19109c2](https://github.com/dbirks/claude-code-proxy/commit/19109c21ff68dd97286f17e2ae425374ddef901a))


### Continuous Integration

* Add publish workflow ([9be47b8](https://github.com/dbirks/claude-code-proxy/commit/9be47b8a7582e6d5c61d8c9c66af5574f1aae67d))
* Add release-please workflow ([41cb03b](https://github.com/dbirks/claude-code-proxy/commit/41cb03befb0d920101b1a24e87e39950df5fbc2c))
* Move renovate.json into .github/ ([94b4805](https://github.com/dbirks/claude-code-proxy/commit/94b48053210fe2c1851671e066c4976687410938))
* Update renovate config file to group deps together ([9c7fd21](https://github.com/dbirks/claude-code-proxy/commit/9c7fd219ae1b993b941228a5286cd2a4cdd53977))


### Dependencies

* Bump package versions and pin them ([79ab6ca](https://github.com/dbirks/claude-code-proxy/commit/79ab6caa1cb3f6eeea000e30d1af0a9e8f197d80))
