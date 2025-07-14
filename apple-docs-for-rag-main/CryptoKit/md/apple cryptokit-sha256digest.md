

- Apple CryptoKit
-  SHA256Digest 

Structure

# SHA256Digest

The output of a Secure Hashing Algorithm 2 (SHA-2) hash with a 256-bit digest.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SHA256Digest
```

## Topics

### Inspecting the digest length

static var byteCount: Int

The number of bytes in the digest.

### Describing a digest

var description: String

A human-readable description of the digest.

### Hashing a digest

func hash(into: inout Hasher)

Hashes the essential components of the digest by feeding them into the given hash function.

## Relationships

### Conforms To

- ContiguousBytes
- Copyable
- CustomStringConvertible
- Digest
- Equatable
- Hashable
- Sendable
- Sequence

## See Also

### Specifying the output type

typealias Digest

The digest type for a SHA256 hash function.

