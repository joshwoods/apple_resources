

- SwiftData
-  DataStoreSnapshotCodingKey 

Enumeration

# DataStoreSnapshotCodingKey

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
enum DataStoreSnapshotCodingKey
```

## Topics

### Enumeration Cases

case modeledProperty(String)

case persistentIdentifier

### Initializers

init?(intValue: Int)

Creates a new instance from the specified integer.

init?(stringValue: String)

Creates a new instance from the given string.

### Instance Properties

var intValue: Int?

The value to use in an integer-indexed collection (e.g. an int-keyed dictionary).

var stringValue: String

The string to use in a named collection (e.g. a string-keyed dictionary).

### Default Implementations

CodingKey Implementations

## Relationships

### Conforms To

- CodingKey
- CustomDebugStringConvertible
- CustomStringConvertible
- Sendable

