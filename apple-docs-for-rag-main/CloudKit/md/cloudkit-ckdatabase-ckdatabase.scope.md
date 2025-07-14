

- CloudKit
- CKDatabase
-  CKDatabase.Scope 

Enumeration

# CKDatabase.Scope

Constants that represent the scope of a database.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum Scope
```

## Topics

### Database Scopes

case `public`

The public database.

case `private`

The private database.

case shared

The shared database.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Database Type

var databaseScope: CKDatabase.Scope

The type of database.

