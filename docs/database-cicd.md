# SQL and Database CI/CD

## Overview

This project uses PostgreSQL and Flyway to manage database schema changes as version-controlled migrations.

The CI/CD database is a dedicated lab database and is not a production database.

## Database Environment

The PostgreSQL database runs on `ltvm07` in the Docker container:

- Container: `springbootlab-postgres`
- PostgreSQL version: 16
- Database: `springbootlab`
- Database user: `springbootlab`
- PostgreSQL container port: 5432
- Host port: 5433
- Host: `172.16.55.177`

The GitHub Actions self-hosted runner runs on `ltvm08`.

Network connectivity was verified from `ltvm08` to `ltvm07`:

```text
172.16.55.177:5433
