

- Apple CryptoKit
-  SymmetricKeySize 

Structure

# SymmetricKeySize

The sizes that a symmetric cryptographic key can take.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SymmetricKeySize
```

## Overview

When creating a new SymmetricKey instance with a call to its init(size:) initializer, you typically use one of the standard key sizes, like bits128, bits192, or bits256. When you need a key with a non-standard length, use the init(bitCount:) initializer to create a `SymmetricKeySize` instance with a custom bit count.

## Topics

### Using standard key lengths

static var bits128: SymmetricKeySize

A size of 128 bits.

static var bits192: SymmetricKeySize

A size of 192 bits.

static var bits256: SymmetricKeySize

A size of 256 bits.

### Creating a nonstandard key length

init(bitCount: Int)

Creates a new key size of the given length.

### Getting the length

let bitCount: Int

The number of bits in the key.

## Relationships

### Conforms To

- Sendable

## See Also

### Message authentication codes

struct HMAC

A hash-based message authentication algorithm.

struct SymmetricKey

A symmetric cryptographic key.

