

- SwiftData
- PersistentIdentifier
-  PersistentIdentifier.ID 

Structure

# PersistentIdentifier.ID

A type that represents the stable identity of a SwiftData model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ID
```

## Topics

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing IDs

static func == (PersistentIdentifier.ID, PersistentIdentifier.ID) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Accessing identity information

let id: PersistentIdentifier.ID

The value that uniquely identifies the associated model within the containing store.

var storeIdentifier: String?

The identifier of the store that contains the associated model.

var entityName: String

The entity name for the associated model.

