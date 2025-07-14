

- Apple CryptoKit
-  SymmetricKey 

Structure

# SymmetricKey

A symmetric cryptographic key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SymmetricKey
```

## Overview

You typically derive a symmetric key from an instance of a shared secret (SharedSecret) that you obtain through key agreement. You use a symmetric key to compute a message authentication code like HMAC, or to open and close a sealed box (ChaChaPoly.SealedBox or AES.GCM.SealedBox) using a cipher like ChaChaPoly or AES.

## Topics

### Creating a key

init&lt;D>(data: D)

Creates a key from the given data.

init(size: SymmetricKeySize)

Generates a new random key of the given size.

### Getting the key length

var bitCount: Int

The number of bits in the key.

## Relationships

### Conforms To

- ContiguousBytes
- Copyable
- Equatable
- Sendable

## See Also

### Message authentication codes

struct HMAC

A hash-based message authentication algorithm.

struct SymmetricKeySize

The sizes that a symmetric cryptographic key can take.

