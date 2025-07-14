

- Apple CryptoKit
- HKDF
-  extract(inputKeyMaterial:salt:) 

Type Method

# extract(inputKeyMaterial:salt:)

Creates cryptographically strong key material from a main key or passcode that you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func extract(
    inputKeyMaterial: SymmetricKey,
    salt: Salt?
) -> HashedAuthenticationCode where Salt : DataProtocol
```

## Parameters 

`inputKeyMaterial`  

The main key or passcode the derivation function uses to derive a key.

`salt`  

The salt to use for key derivation.

## Return Value

A pseudorandom, cryptographically strong key in the form of a hashed authentication code.

## Discussion

Generate a derived symmetric key from the cryptographically strong key material this function creates by calling expand(pseudoRandomKey:info:outputByteCount:).

## See Also

### Controlling key derivation

static func expand&lt;PRK, Info>(pseudoRandomKey: PRK, info: Info?, outputByteCount: Int) -> SymmetricKey

Expands cryptographically strong key material into a derived symmetric key.

