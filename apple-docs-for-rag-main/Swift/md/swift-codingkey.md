

- Swift
-  CodingKey 

Protocol

# CodingKey

A type that can be used as a key for encoding and decoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol CodingKey : CustomDebugStringConvertible, CustomStringConvertible, Sendable
```

## Topics

### Initializers

init?(intValue: Int)

Creates a new instance from the specified integer.

**Required**

init?(stringValue: String)

Creates a new instance from the given string.

**Required**

### Instance Properties

var intValue: Int?

The value to use in an integer-indexed collection (e.g. an int-keyed dictionary).

**Required**

var stringValue: String

The string to use in a named collection (e.g. a string-keyed dictionary).

**Required**

## Relationships

### Inherits From

- CustomDebugStringConvertible
- CustomStringConvertible
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

protocol CodingKeyRepresentable

A type that can be converted to and from a coding key.

struct CodingUserInfoKey

A user-defined key for providing context during encoding and decoding.

