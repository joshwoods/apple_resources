

- Apple CryptoKit
- HPKEPublicKeySerialization
-  init(\_:kem:) 

Initializer

# init(\_:kem:)

Creates a public key from an encoded representation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    _ serialization: D,
    kem: HPKE.KEM
) throws where D : ContiguousBytes
```

**Required**

## Discussion

- serialization: The serialized key data.

- kem: The key encapsulation mechanism that the sender used to encapsulate the key.

