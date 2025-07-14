

- Apple CryptoKit
-  MessageAuthenticationCode 

Protocol

# MessageAuthenticationCode

A type that represents a message authentication code.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
protocol MessageAuthenticationCode : ContiguousBytes, CustomStringConvertible, Hashable, Sendable, Sequence where Self.Element == UInt8
```

## Topics

### Retrieving the code length

var byteCount: Int

The number of bytes in the message authentication code.

**Required**

### Comparing codes

static func == &lt;D>(Self, D) -> Bool

Returns a Boolean value indicating whether a message authentication code is equivalent to a collection of binary data.

static func == (Self, Self) -> Bool

Returns a Boolean value indicating whether two message authentication codes are equal.

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Inherits From

- ContiguousBytes
- CustomStringConvertible
- Equatable
- Hashable
- Sendable
- Sequence

### Conforming Types

- HashedAuthenticationCode

## See Also

### Working with codes

typealias MAC

An alias for a hash-based message authentication code.

struct HashedAuthenticationCode

A hash-based message authentication code.

