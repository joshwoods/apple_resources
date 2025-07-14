

- Apple CryptoKit
- AES
- AES.GCM
-  AES.GCM.Nonce 

Structure

# AES.GCM.Nonce

A value used once during a cryptographic operation and then discarded.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Nonce
```

## Overview

Don’t reuse the same nonce for multiple calls to encryption APIs. It’s critical that nonces are unique per call to encryption APIs in order to protect the integrity of the encryption.

## Topics

### Creating a nonce

init()

Creates a new random nonce.

init&lt;D>(data: D) throws

Creates a nonce from the given data.

### Iterating over a nonce’s bytes

func makeIterator() -> Array&lt;UInt8>.Iterator

Returns an iterator over the elements of the nonce.

## Relationships

### Conforms To

- ContiguousBytes
- Sendable
- Sequence

