# Changelog

All notable changes to the Qanapi documentation site (https://docs.qanapi.com) are documented in this file. Versions up to 1.2.1 were assigned from the commit history when this file was created on 2026-10-13, and each of those dates is the date of the last commit in that release.

## [1.3.0] - 2026-10-13

### Added

- This changelog, following the Qanapi changelog rules.
- Release announcements in Slack. After each push to `main`, the `release-announcement.yml` workflow waits for Mintlify to finish, then asks IntegrationManager to announce the newest release in this changelog. A failed Mintlify deployment is not announced.

## [1.2.1] - 2026-10-01

### Changed

- Every change is now checked for broken links, anchors, snippets, and redirects, and for a valid Mintlify configuration, by a pre-commit hook and by the "Docs check" GitHub Actions workflow before it is merged.

### Fixed

- Broken links on the introduction page, the API v3 overview and headers pages, and the Standalone API v3 pages.

## [1.2.0] - 2026-09-28

Qanapi Flow gains purchasing, guided setup, and live redaction guides, and the API reference adds the self-hosted Standalone API v3.

### Added

- Live Redaction guide, with screenshots for converting existing integrations to the new URLs.
- "Purchasing Qanapi Flow" guide.
- Guided Setup guide for getting started with a Qanapi Flow bundle.
- Standalone API v3 reference ("3.x - Stand Alone"), covering the self-hosted service: encryption, classifications, policies, authentication, users, configurations, API keys, health, KMS, audit, and transport, with overview and custom headers pages.

### Changed

- Updated the dark theme logo.

## [1.1.0] - 2026-08-19

### Added

- Classifications endpoints in the API v3 reference (list, view, create, update, and delete).
- Classifications page in Get Started, explaining how classifications secure data.
- Classification header details on the API v3 custom headers page.

### Changed

- The API v2 and v3 references now come from one OpenAPI specification, and API v3 routes are shown with their `/v3/` prefix.

### Fixed

- A broken link on the API v2 custom headers page.

## [1.0.0] - 2026-07-31

The documentation is rebuilt around the API, with separate Documentation and API Reference tabs and an OpenAPI based reference for every API version.

### Added

- Documentation and API Reference tabs, with a version switcher for API 3.x, 2.x, and 1.x.
- OpenAPI based API reference for v1, v2, and v3, with request and response examples and error details.
- API v3 endpoints for encryption, roles, users, configurations, API keys, and logs, including pagination details.
- Get Started section with a new introduction, quickstart, and Configurations page.
- Overview and custom headers pages for each API version.
- SDKs page with the official SDKs and client libraries.
- S/MIME guide, with setup help and troubleshooting.

### Changed

- The quickstart explains where to find the API key for the `X-Qanapi-Authorization` header and the proxy slug used by the encrypt and decrypt routes.
- Encryption containers are now called configurations throughout the documentation.
- The encrypt and decrypt references explain dot notation for nested fields, the maximum JSON depth of 32, and that the fields to decrypt are required.
- API v1 responses now match the actual API.
- New fonts, scrollbar styling, and route alignment in the sidebar.

### Removed

- **Breaking:** The original guide pages (registration, dashboard navigation, creating projects, project management, administration, and the data proxy guides and examples) were removed in favor of the new Get Started pages and API reference. Links to those pages no longer work.

## [0.2.1] - 2026-04-22

### Changed

- Removed icons from the API v2 pages.

### Removed

- Data classifications from the API v1 data proxy pages and from the cURL, JavaScript, and Python examples.

## [0.2.0] - 2025-07-30

### Added

- API v2 documentation: quick start, setup, authentication, encryption, decryption, links, and security, with OpenAPI specifications.

### Changed

- The data proxy guides and the cURL, JavaScript, and Python examples moved to a separate API v1 section.
- Updated the introduction, quickstart, API keys, data classifications, and project pages for API v2.

## [0.1.0] - 2025-03-25

### Added

- First version of the documentation site, built on Mintlify with Qanapi branding.
- Getting started guides: registration, dashboard navigation, and creating projects.
- Project management guides: overview, API keys, and data classifications.
- Administration guides: billing, security logging, settings, and team management.
- Data proxy guides for encryption, decryption, and forwarding, with cURL, JavaScript, and Python examples.
