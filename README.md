# ToastCore
ToastCore is an updated version of the unofficial [2018 LambdaCore database](https://lisdude.com/moo/LambdaCore-20Jun18.db.gz). It's intended either as a replacement for LambdaCore when starting a new MOO or as a reference for implementing ToastStunt-specific features in existing databases.

## Features
- Updated core utility verbs with ToastStunt equivalents where appropriate
- ANSI 2.5
- MCP 2.1
- Replace crypt() with Argon2id password hashing
- Skeleton waif and anonymous objects
- Various builtin type prototypes that redirect to their $generic_utils counterparts
    - e.g. `"My cool string":explode()`
- Stunt Shapes object serializer
- MCP SimpleEdit updates
    - Support for lists
    - Support for //-style comments
- Inline editor used on ChatMUD and Miriani (previously known as 'Flexible Editor')
- Poor man's namespaces
    - Maps on #0 can be expanded when matching
    - e.g. `@edit $help_db["toaststunt"].argon2`
- $recycler that uses recycle() and recreate() instead of $garbage objects
- Network name lookups handled in-database in a separate thread
- General cleanup of antiquated / unused things in LambdaCore

An exhaustive list of changes can be found in the [changelog](changelog.txt).

## Requirements
- [ToastStunt v2.6.0 or later](https://github.com/lisdude/toaststunt)
