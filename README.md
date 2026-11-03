# pg_store_plans — Windows x64

[日本語](README_ja.md) | English

This repository provides **unofficial Windows x64 binaries** for [pg_store_plans](https://github.com/ossc-db/pg_store_plans). SQL execution plan statistics for PostgreSQL.

## Download and compatibility

Get the [latest published Release](https://github.com/pgextwin/pg_store_plans/releases/latest) or [browse all Releases](https://github.com/pgextwin/pg_store_plans/releases). Published packages for PostgreSQL **14–18** are listed in the [pgextwin catalog](https://pgextwin.github.io/website/en/). Download the ZIP matching your PostgreSQL major version. PostgreSQL 14 community support ends November 12, 2026; historical downloads may remain available.

## Installation

1. Back up your PostgreSQL environment and check [upstream installation requirements](https://github.com/ossc-db/pg_store_plans).
2. Stop PostgreSQL before replacing files. Extract the ZIP for your PostgreSQL major and copy the packaged lib/ and share/extension/ files into the matching PostgreSQL installation directories.
3. Add pg_store_plans to shared_preload_libraries in postgresql.conf, following the upstream documentation. Start or restart PostgreSQL.
4. Run CREATE EXTENSION pg_store_plans; in the database where the extension is needed.

Verify downloaded files using SHA256SUMS.txt from the Release. Review the Release for SPDX SBOMs, vulnerability reports and signed attestations. Test in a non-production environment before deployment.

## License and support

Consult [upstream pg_store_plans](https://github.com/ossc-db/pg_store_plans) for SQL usage, settings, permissions, and limitations. pgextwin is an independent community package and is not an official upstream distribution. Refer to the included license.
