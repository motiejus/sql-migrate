# sql-migrate

A direct fork of github.com/quarksgroup/sql-migrate, which itself is a fork of
github.com/rubenv/sql-migrate. Main differences:

- add `go:embed` support (from quarksgroup, no changes mine)
- remove support for everything but sqlite.
- vendor `gorp`, so it does not pull in unnecessary dependencies.
- remove integration tests and a few unit tests, which were bringing in
  dependencies.
