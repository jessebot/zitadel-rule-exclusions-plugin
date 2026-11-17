# OWASP CRS - Zitadel Rule Exclusions Plugin

![Integration tests](https://github.com/coreruleset/zitadel-rule-exclusions-plugin/actions/workflows/integration.yml/badge.svg)

This is a 3rd party OWASP CRS Rule Exclusions Plugin for users running Zitadel, an IDP with OIDC and Oauth2 capabilities.

This repo lives at [git.open.engineering](https://git.open.engineering/oeng/zitadel-rule-exclusions-plugin) but is mirrored to the following locations:
- [Codeberg](https://codeberg.org/open-engineering/zitadel-rule-exclusions-plugin)
- [GitHub](https://github.com/jessebot/zitadel-rule-exclusions-plugin)

The CRS plugin documentation can be found on the [website](https://coreruleset.org/docs/configuring/plugins/).

## Testing

Plugins can also be shipped with their own tests. Any `ftw` test yaml file that you add below the `tests/regression` directory will be run by the integrated pipeline.
We suggest you to use a new subdirectory for your specific plugin's test, e.g. `tests/regression/<your-plugin>`, and create one file per rule you want to test.

Many plugins target rule exclusions, so it will be rather common to see tests matching a REQUEST_URI but matching for `no_log_contains`, as we want to test that we are not being blocked.

## License

Copyright (c) 2021-2022 OWASP CRS project. All rights reserved.

The OWASP CRS and its official plugins are
distributed under Apache Software License (ASL) version 2.
Please see the enclosed LICENSE file for full details.
