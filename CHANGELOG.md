## [1.0.1](https://github.com/WYRE-AI/node-clio/compare/v1.0.0...v1.0.1) (2026-08-25)


### Bug Fixes

* migrate to WYRE-AI org (npm scope, ghcr namespace, registry) ([#1](https://github.com/WYRE-AI/node-clio/issues/1)) ([eb85536](https://github.com/WYRE-AI/node-clio/commit/eb85536879025ed892177377c04951d92b29374f))

# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-07-15

### Added

- Initial release of `@wyre-ai/node-clio`, a TypeScript/JavaScript client
  for the Clio Manage API v4.
- Region-aware `ClioClient` supporting US, EU, CA, and AU deployments.
- OAuth 2.0 authorization-code and refresh-token flows (`src/auth.ts`).
- Automatic access-token refresh on `401` responses when refresh credentials are
  configured.
- Resources: `matters`, `contacts`, `activities`, `communications` (read-only),
  `tasks`, `documents` (metadata only), `calendarEntries` (read-only), `bills`
  (read-only).
- Typed error hierarchy: `ServiceError`, `AuthenticationError`, `ForbiddenError`,
  `NotFoundError`, `ValidationError`, `RateLimitError`, `ServerError`.
- Zero runtime dependencies (native `fetch` only).

### Features

- initial Clio Manage API v4 TypeScript SDK ([cc30c81](https://github.com/WYRE-AI/node-clio/commit/cc30c8158ac96f4e513db1f78a3ce02c036db8a0))

[Unreleased]: https://github.com/WYRE-AI/node-clio/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/WYRE-AI/node-clio/releases/tag/v1.0.0
