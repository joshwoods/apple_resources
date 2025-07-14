

- Swift
-  CodingUserInfoKey 

Structure

# CodingUserInfoKey

A user-defined key for providing context during encoding and decoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CodingUserInfoKey
```

## Topics

### Operators

static func == (CodingUserInfoKey, CodingUserInfoKey) -> Bool

Returns a Boolean value indicating whether the given keys are equal.

### Initializers

init?(rawValue: String)

Creates a new instance with the given raw value.

### Instance Properties

var hashValue: Int

The key’s hash value.

let rawValue: String

The key’s string value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let actorSystemKey: CodingUserInfoKey

Key which is required to be set on a `Decoder`’s `userInfo` while attempting to `init(from:)` a `DistributedActor`. The stored value under this key must conform to `DistributedActorSystem`.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Custom Encoding and Decoding

Encoding and Decoding Custom Types

Make your data types encodable and decodable for compatibility with external representations such as JSON.

typealias Codable

A type that can convert itself into and out of an external representation.

protocol Encodable

A type that can encode itself to an external representation.

protocol Decodable

A type that can decode itself from an external representation.

protocol CodingKey

A type that can be used as a key for encoding and decoding.

protocol CodingKeyRepresentable

A type that can be converted to and from a coding key.

