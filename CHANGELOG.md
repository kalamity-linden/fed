## v0.3.0 (Released 2019-08-16)

BREAKING CHANGES

We've renamed all OpenAPI fields like `Id` to `ID` to be consistent with Go's style.

ADDITIONS

- add environment variables to override command line flags (`LOG_FORMAT`, `HTTP_BIND_ADDRESS`, `HTTP_ADMIN_BIND_ADDRESS`)
- cmd/server: bind HTTP server with TLS if HTTPS_* variables are defined

IMPROVEMENTS

- docs: update docs.moov.io links after design refresh
- docs: link to app specific docs.moov.io page
- cmd/server: quit with an exit code of 1 on missing data files

BUILD

- chore(deps): update module prometheus/client_golang to v1.1.0
- build: download tools used by TravisCI instead of installing them

## v0.2.0 (Released 2019-06-19)

BUILD

- Ship old example FED data files in the Docker image. Production deployments need to replace these with updated files from their Financial Institution.

## v0.1.x (Released 2019-03-06)

BUG FIXES

- Fix automated build steps and Docker setup

ADDITIONS

- Added environmental variables for data filepaths

## v0.1.0 (Released 2019-03-06)

- Initial release
