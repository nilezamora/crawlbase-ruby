# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.0] - 2026-07-14

### Added

- `cb_status` reader on `Crawlbase::API` and `Crawlbase::StorageAPI` responses. Parsing prefers `cb_status` from the HTTP/JSON response and falls back to `pc_status` for compatibility with older API responses.

### Deprecated

- `pc_status` is deprecated in favor of `cb_status`. It remains available as an alias and emits a deprecation warning when called. It will be removed in a future major release.
