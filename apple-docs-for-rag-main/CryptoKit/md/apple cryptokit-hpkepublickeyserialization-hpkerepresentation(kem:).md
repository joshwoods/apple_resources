

- Apple CryptoKit
- HPKEPublicKeySerialization
-  hpkeRepresentation(kem:) 

Instance Method

# hpkeRepresentation(kem:)

Creates an encoded representation of the public key.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func hpkeRepresentation(kem: HPKE.KEM) throws -> Data
```

**Required**

## Return Value

The encoded key data.

## Discussion

- kem: The key encapsulation mechanism for encapsulating the key.

