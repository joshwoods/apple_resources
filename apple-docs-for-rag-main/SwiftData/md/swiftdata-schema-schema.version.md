

- SwiftData
- Schema
-  Schema.Version 

Structure

# Schema.Version

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
struct Version
```

## Topics

### Operators

static func == (Schema.Version, Schema.Version) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (Schema.Version, Schema.Version) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Initializers

init(Int, Int, Int)

Initializes a version struct with the provided components of a semantic version.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var description: String

A textual description of the version object.

var hashValue: Int

The hash value.

let major: Int

The major version according to the semantic versioning standard.

let minor: Int

The minor version according to the semantic versioning standard.

let patch: Int

The patch version according to the semantic versioning standard.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable

