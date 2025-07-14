

- Apple CryptoKit
-  Digest 

Protocol

# Digest

A type that represents the output of a hash.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
protocol Digest : ContiguousBytes, CustomStringConvertible, Hashable, Sendable, Sequence where Self.Element == UInt8
```

## Topics

### Getting the digest length

static var byteCount: Int

The number of bytes in the digest.

**Required**

### Comparing digests

static func == &lt;D>(Self, D) -> Bool

Determines whether a digest is equivalent to a collection of contiguous bytes.

static func == (Self, Self) -> Bool

Determines whether two digests are equal.

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

- Insecure.MD5Digest
- Insecure.SHA1Digest
- SHA256Digest
- SHA384Digest
- SHA512Digest

## See Also

### Specifying the output type

associatedtype Digest : Digest

**Required**

