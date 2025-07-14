

- Apple CryptoKit
- HKDF
-  expand(pseudoRandomKey:info:outputByteCount:) 

Type Method

# expand(pseudoRandomKey:info:outputByteCount:)

Expands cryptographically strong key material into a derived symmetric key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func expand(
    pseudoRandomKey prk: PRK,
    info: Info?,
    outputByteCount: Int
) -> SymmetricKey where PRK : ContiguousBytes, Info : DataProtocol
```

## Parameters 

`prk`  

A pseudorandom, cryptographically strong key generated from the extract(inputKeyMaterial:salt:) function.

`info`  

The shared information to use for key derivation.

`outputByteCount`  

The length in bytes of the resulting symmetric key.

## Return Value

The derived symmetric key.

## Discussion

Generate cryptographically strong key material to use with this function by calling extract(inputKeyMaterial:salt:).

## See Also

### Controlling key derivation

static func extract&lt;Salt>(inputKeyMaterial: SymmetricKey, salt: Salt?) -> HashedAuthenticationCode&lt;H>

Creates cryptographically strong key material from a main key or passcode that you specify.

