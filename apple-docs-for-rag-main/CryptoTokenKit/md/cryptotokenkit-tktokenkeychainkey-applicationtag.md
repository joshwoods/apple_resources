

- CryptoTokenKit
- TKTokenKeychainKey
-  applicationTag 

Instance Property

# applicationTag

The private tag data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var applicationTag: Data? { get set }
```

## Discussion

This property is equivalent to the `kSecAttrApplicationTag` type attribute.

## See Also

### Accessing Key Attributes

var keyType: String

The type of the key. Currently, only kSecAttrKeyTypeRSA and `kSecAttrKeyTypeECSECPrimeRandom` are supported values.

var keySizeInBits: Int

var publicKeyData: Data?

The public key data.

var publicKeyHash: Data?

The SHA1 hash of the raw public key.

var canDecrypt: Bool

Whether the key can be used to decrypt data.

var canSign: Bool

Whether the key can be used to sign data.

var canPerformKeyExchange: Bool

Whether the key can be used to perform Diffie-Hellman style cryptographic key exchange.

var isSuitableForLogin: Bool

Whether the key can be used for system login.

