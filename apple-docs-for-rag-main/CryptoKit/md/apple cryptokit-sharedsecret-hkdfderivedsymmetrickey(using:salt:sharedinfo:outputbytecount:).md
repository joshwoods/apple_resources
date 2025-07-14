

- Apple CryptoKit
- SharedSecret
-  hkdfDerivedSymmetricKey(using:salt:sharedInfo:outputByteCount:) 

Instance Method

# hkdfDerivedSymmetricKey(using:salt:sharedInfo:outputByteCount:)

Derives a symmetric encryption key from the secret using HKDF key derivation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func hkdfDerivedSymmetricKey(
    using hashFunction: H.Type,
    salt: Salt,
    sharedInfo: SI,
    outputByteCount: Int
) -> SymmetricKey where H : HashFunction, Salt : DataProtocol, SI : DataProtocol
```

## Parameters 

`hashFunction`  

The hash function to use for key derivation.

`salt`  

The salt to use for key derivation.

`sharedInfo`  

The shared information to use for key derivation.

`outputByteCount`  

The length in bytes of resulting symmetric key.

## Return Value

The derived symmetric key.

## See Also

### Deriving keys

func x963DerivedSymmetricKey&lt;H, SI>(using: H.Type, sharedInfo: SI, outputByteCount: Int) -> SymmetricKey

Derives a symmetric encryption key from the secret using x9.63 key derivation.

