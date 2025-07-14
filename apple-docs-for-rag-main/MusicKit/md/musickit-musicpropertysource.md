

- MusicKit
-  MusicPropertySource 

Enumeration

# MusicPropertySource

An enumeration that specifies which source to use when requesting properties and relationships.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum MusicPropertySource
```

## Topics

### Operators

static func == (MusicPropertySource, MusicPropertySource) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case catalog

The source representing the Apple Music catalog.

case library

The source representing the user’s music library.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

### Type Properties

static var allCases: [MusicPropertySource]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

