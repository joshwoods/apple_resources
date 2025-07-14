

- Apple CryptoKit
- HKDF
-  deriveKey(inputKeyMaterial:salt:info:outputByteCount:) 

Type Method

# deriveKey(inputKeyMaterial:salt:info:outputByteCount:)

Derives a symmetric encryption key from a main key or passcode using HKDF key derivation with information and salt you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func deriveKey(
    inputKeyMaterial: SymmetricKey,
    salt: Salt,
    info: Info,
    outputByteCount: Int
) -> SymmetricKey where Salt : DataProtocol, Info : DataProtocol
```

## Parameters 

`inputKeyMaterial`  

The main key or passcode the derivation function uses to derive a key.

`salt`  

The salt to use for key derivation.

`info`  

The shared information to use for key derivation.

`outputByteCount`  

The length in bytes of the resulting symmetric key.

## Return Value

The derived symmetric key.

## See Also

### Deriving a key

static func deriveKey(inputKeyMaterial: SymmetricKey, outputByteCount: Int) -> SymmetricKey

Derives a symmetric encryption key from a main key or passcode using HKDF key derivation.

static func deriveKey&lt;Info>(inputKeyMaterial: SymmetricKey, info: Info, outputByteCount: Int) -> SymmetricKey

Derives a symmetric encryption key from a main key or passcode using HKDF key derivation with information you specify.

static func deriveKey&lt;Salt>(inputKeyMaterial: SymmetricKey, salt: Salt, outputByteCount: Int) -> SymmetricKey

Derives a symmetric encryption key from a main key or passcode using HKDF key derivation with salt that you specify.

