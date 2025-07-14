

- Apple CryptoKit
-  HashedAuthenticationCode 

Structure

# HashedAuthenticationCode

A hash-based message authentication code.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct HashedAuthenticationCode where H : HashFunction
```

## Topics

### Retrieving the code length

var byteCount: Int

The number of bytes in the message authentication code.

### Describing a code

var description: String

A human-readable description of the code.

## Relationships

### Conforms To

- ContiguousBytes
- CustomStringConvertible
- Equatable
- Hashable
- MessageAuthenticationCode
- Sendable
- Sequence

## See Also

### Working with codes

typealias MAC

An alias for a hash-based message authentication code.

protocol MessageAuthenticationCode

A type that represents a message authentication code.

