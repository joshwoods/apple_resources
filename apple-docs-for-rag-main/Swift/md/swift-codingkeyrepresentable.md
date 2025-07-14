

- Swift
-  CodingKeyRepresentable 

Protocol

# CodingKeyRepresentable

A type that can be converted to and from a coding key.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
protocol CodingKeyRepresentable
```

## Overview

With a `CodingKeyRepresentable` type, you can losslessly convert between a custom type and a `CodingKey` type.

Conforming a type to `CodingKeyRepresentable` lets you opt in to encoding and decoding `Dictionary` values keyed by the conforming type to and from a keyed container, rather than encoding and decoding the dictionary as an unkeyed container of alternating key-value pairs.

## Topics

### Initializers

init?&lt;T>(codingKey: T)

**Required**

### Instance Properties

var codingKey: any CodingKey

**Required**

## Relationships

### Conforming Types

- Int
- String

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

struct CodingUserInfoKey

A user-defined key for providing context during encoding and decoding.

