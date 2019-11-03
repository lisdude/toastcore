# ToastCore
ToastCore is an updated version of the [2018 LambdaCore database](https://lisdude.com/moo/LambdaCore-20Jun18.db.gz). It's intended either as a replacement for LambdaCore when starting a new MOO or as a reference for implementing ToastStunt-specific features in existing databases.

## Features
- Updated core verbs with ToastStunt equivalents where appropriate
- ANSI 2.5
- MCP 2.1
- Argon2id password hashing by default
- Skeleton waif and anonymous objects
- Various builtin type prototypes
    - e.g. `"My cool string":explode()`
- Stunt Composed package manager
- Stunt Shapes object serializer
- MCP SimpleEdit support for lists and //-style comments
- Inline editor used on ChatMUD and Miriani (previously known as 'Flexible Editor')
- Poor man's namespaces
    - Maps on #0 can be expanded when matching
    - e.g. `@edit $help_db["toaststunt"].argon2`
- $recycler that uses recycle() and recreate() instead of $garbage objects
- General cleanup of antiquated / unused things in LambdaCore

An exhaustive list of changes can be found in the [changelog](changelog.txt).
