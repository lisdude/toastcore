# Contributing

## Acceptable Changes
* Bug fixes
* Performance enhancements
* Improvements that are of value to everyone

## Backwards Compatibility
* Try to maintain backwards compatibility where possible

## Making a core database

1. Ensure the MOO is compiled with outbound network connections disabled
2. Load the MOO with toastcore.db
3. Make your changes
4. As `wizard` run the verb `make-core-database`
5. After the database is dumped, move it into the `toastcore` repo and rename it to `toastcore.db`
6. Update the changelog with your updates
7. Open a Pull Request describing your changes
