

- SwiftData
-  PersistentIdentifier 

Structure

# PersistentIdentifier

A type that describes the aggregate identity of a SwiftData model.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct PersistentIdentifier
```

## Overview

Note

Decoded PersistentIdentifier and identifiers created by the DefaultStore are not considered equivalent.

## Topics

### Accessing identity information

let id: PersistentIdentifier.ID

The value that uniquely identifies the associated model within the containing store.

struct ID

A type that represents the stable identity of a SwiftData model.

var storeIdentifier: String?

The identifier of the store that contains the associated model.

var entityName: String

The entity name for the associated model.

### Encoding and decoding

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing identifiers

static func == (PersistentIdentifier, PersistentIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (PersistentIdentifier, PersistentIdentifier) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Instance Properties

var hashValue: Int

The hash value.

### Type Methods

static func identifier&lt;T>(for: String, entityName: String, primaryKey: T) throws -> PersistentIdentifier

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Decodable
- Encodable
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Identifying the model instance

var persistentModelID: PersistentIdentifier

var modelContext: ModelContext?

