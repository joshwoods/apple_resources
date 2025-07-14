

- Apple CryptoKit
- SharedSecret
-  x963DerivedSymmetricKey(using:sharedInfo:outputByteCount:) 

Instance Method

# x963DerivedSymmetricKey(using:sharedInfo:outputByteCount:)

Derives a symmetric encryption key from the secret using x9.63 key derivation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func x963DerivedSymmetricKey(
    using hashFunction: H.Type,
    sharedInfo: SI,
    outputByteCount: Int
) -> SymmetricKey where H : HashFunction, SI : DataProtocol
```

## Parameters 

`hashFunction`  

The hash function to use for key derivation.

`sharedInfo`  

The shared information to use for key derivation.

`outputByteCount`  

The length in bytes of resulting symmetric key.

## Return Value

The derived symmetric key.

## See Also

### Deriving keys

func hkdfDerivedSymmetricKey&lt;H, Salt, SI>(using: H.Type, salt: Salt, sharedInfo: SI, outputByteCount: Int) -> SymmetricKey

Derives a symmetric encryption key from the secret using HKDF key derivation.

