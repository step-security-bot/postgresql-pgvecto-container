# PostgreSQL with pgvecto.rs Container

[![](https://img.shields.io/github/license/muhlba91/postgresql-pgvecto-container?style=for-the-badge)](LICENSE)
[![](https://img.shields.io/github/actions/workflow/status/muhlba91/postgresql-pgvecto-container/release.yml?style=for-the-badge)](https://github.com/muhlba91/postgresql-pgvecto-container/actions/workflows/release.yml)
[![](https://img.shields.io/github/v/tag/muhlba91/postgresql-pgvecto-container?style=for-the-badge)](https://github.com/muhlba91/postgresql-pgvecto-container/releases)
[![](https://img.shields.io/github/release-date/muhlba91/postgresql-pgvecto-container?style=for-the-badge)](https://github.com/muhlba91/postgresql-pgvecto-container/releases)
<a href="https://www.buymeacoffee.com/muhlba91" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="28" width="150"></a>

A container integrating [pgvecto.rs](https://github.com/tensorchord/pgvecto.rs) into [CloudNativePG's PostgreSQL container](https://github.com/cloudnative-pg/postgres-containers).

---

> [!WARNING]
> **This container is based on personal needs, in particular its usage with [Immich](https://immich.app)!**
> The chosen upstream versions follow the [Immich requirements](https://github.com/immich-app/immich/blob/main/docker/docker-compose.yml).

---

## Installation Notes

Instead of using the upstream [CloudNativePG container](https://github.com/cloudnative-pg/postgres-containers/pkgs/container/postgresql) you plug in `ghcr.io/muhlba91/postgresql-pgvecto:<TAG>`.

### Container Tags

The container images are tagged according to CloudNativePG's [image tag requirements](https://cloudnative-pg.io/documentation/1.23/container_images/#image-tag-requirements_1).
Additionally, `latest` and `<GIT_COMMIT_SHA>` tags are created which are **not** compatible with CloudNativePG!

The tagging scheme is `<CLOUDNATIVEPG_POSTGRESQL_TAG>-<PGVECTO_TAG>[-<RELEASE_TAG>]` with:

- `<CLOUDNATIVEPG_POSTGRESQL_TAG>`: the upstream [CloudNativePG container](https://github.com/cloudnative-pg/postgres-containers/pkgs/container/postgresql) version
- `<PGVECTO_TAG>`: the [pgvecto.rs](https://github.com/tensorchord/pgvecto.rs/releases) version
- `<RELEASE_TAG>`: the release version of this container (used to version internal changes; optional to specify)

---

## Contributing

We welcome community contributions to this project.

## Supporting

If you enjoy the application and want to support my efforts, please feel free to buy me a coffe. :)

<a href="https://www.buymeacoffee.com/muhlba91" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="75" width="300"></a>
