

- Apple CryptoKit
- Insecure
-  Insecure.SHA1 

Structure

# Insecure.SHA1

An implementation of SHA1 hashing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SHA1
```

## Overview

The Insecure.SHA1 hash implements the HashFunction protocol to produce a SHA1 digest (Insecure.SHA1Digest).

You can compute the digest by calling the static `hash(data:)` method once. Alternatively, if the data that you want to hash is too large to fit in memory, you can compute the digest iteratively by creating a new hash instance, calling the `update(data:)` method repeatedly with blocks of data, and then calling the finalize() method to get the result.

Important

This hash algorithm isn’t considered cryptographically secure, but is provided for backward compatibility with older services that require it. For new services, prefer one of the secure hashes, like SHA512.

## Topics

### Specifying the output type

typealias Digest

The digest type for a SHA1 hash function.

struct SHA1Digest

The output of a SHA1 hash.

### Reporting the hash length

static let byteCount: Int

The number of bytes in a SHA1 digest.

### Computing a hash iteratively

init()

Creates a SHA1 hash function.

func update(bufferPointer: UnsafeRawBufferPointer)

Incrementally updates the hash function with the contents of the buffer.

func finalize() -> Insecure.SHA1.Digest

Finalizes the hash function and returns the computed digest.

### Reporting hash function information

static let blockByteCount: Int

The number of bytes that represents the hash function’s internal state.

## Relationships

### Conforms To

- Copyable
- HashFunction
- Sendable

## See Also

### Hashes

struct MD5

An implementation of MD5 hashing.

