# RingCentral Engage API Docs

[![Build Status][build-status-svg]][build-status-link]
[![Docs Status][docs-status-svg]][docs-status-link]
[![Docs][docs-svg]][docs-link]

This repository is the home of the RingCentral Engage Developer Guide: a collection of materials, and documentation to help educate developers on how to build on top of the RingCentral Engage platform.

Visit a [live preview][docs-link] of https://developers.ringcentral.com/engage/digital/guide

## Contributing

If you would like to contribute to the RingCentral documentation effort, fork this repository, make your desired edits and contributions, and issue a pull request accordingly.

### Running ReadTheDocs Locally

```
% git clone https://github.com/ringcentral/engage-digital-api-docs.git
% cd engage-digital-api-docs
% pip install mkdocs
% pip install mkdocs-ringcentral
% mkdocs serve
```

Then you should be able to load http://localhost:8000 to view the documentation.

### Testing OpenAPI Specs

This repo holds OpenAPI specs for Engage Digital. 

You can preview the latest version of the swagger spec on the [swagger preview][swagger-preview]

For each commit, tests are run on Travis CI to verify that the OpenAPI 3.0 specs validate.

* Engage Digital Spec: [specs/digital/engage-digital_openapi3.yaml](specs/engage-digital_openapi3.yaml)
* Tests: [specs_test.go](specs_test.go)

You can verify the specs localy with the following if you have [Go installed](https://golang.org/).

```
% git clone https://github.com/ringcentral/ringcentral-api-docs.git
% cd ringcentral-api-docs
% go test -v ./...
```

If you wish to change the specs being tested edit the [specs_test.go](specs_test.go) file.

 [build-status-svg]: https://api.travis-ci.com/ringcentral/engage-digital-api-docs.svg?branch=master
 [build-status-link]: https://travis-ci.com/github/ringcentral/engage-digital-api-docs
 [docs-status-svg]: https://readthedocs.org/projects/engage-digital-api-docs/badge/?version=latest
 [docs-status-link]: https://readthedocs.org/projects/engage-digital-api-docs/builds/
 [docs-svg]: https://img.shields.io/badge/docs-readthedocs-blue.svg
 [docs-link]: https://engage-digital-api-docs.readthedocs.io/en/latest/
 [swagger-preview]: https://ringcentral.github.io/engage-digital-api-docs/digital/
