# Secure EcmaScript (SES)

Secure EcmaScript is a frozen environment for running EcmaScript 'strict'
mode programs. These programs run without ambient authority in their global
scope, and add safe two-argument evaluator (`SES.confine(code, endowments)`)
to each realm. It runs atop an ES6-compliant platform, enabling safe
interaction of mutually-suspicious code, using object-capabilities.

See https://github.com/Agoric/TinySES to see how SES fits into the various
flavors of confined EcmaScript execution.

Build a Secure EcmaScript (SES) environment

Derived from the Caja project, https://github.com/google/caja/wiki/SES .

Still under development: do not use for production systems yet, there are
known security holes that need to be closed.

Incorporates (as a git submodule) the Realms shim from
https://github.com/tc39/proposal-realms .

### Project Badges

[![Build Status][travis-svg]][travis-url]
<!-- [![Coverage Status][coveralls-svg]][coveralls-url] -->
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]

[travis-svg]: https://travis-ci.com/Agoric/SES.svg?branch=master
[travis-url]: https://travis-ci.com/Agoric/SES
[coveralls-svg]: https://coveralls.io/repos/github/Agoric/SES/badge.svg
[coveralls-url]: https://coveralls.io/github/Agoric/SES
[deps-svg]: https://david-dm.org/Agoric/SES.svg
[deps-url]: https://david-dm.org/Agoric/SES
[dev-deps-svg]: https://david-dm.org/Agoric/SES/dev-status.svg
[dev-deps-url]: https://david-dm.org/Agoric/SES?type=dev
[license-image]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
[license-url]: shim/LICENSE