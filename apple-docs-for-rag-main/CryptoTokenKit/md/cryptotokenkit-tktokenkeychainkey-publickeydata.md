

- CryptoTokenKit
- TKTokenKeychainKey
-  publicKeyData 

Instance Property

# publicKeyData

The public key data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var publicKeyData: Data? { get set }
```

## See Also

### Accessing Key Attributes

var keyType: String

The type of the key. Currently, only kSecAttrKeyTypeRSA and `kSecAttrKeyTypeECSECPrimeRandom` are supported values.

var keySizeInBits: Int

var applicationTag: Data?

The private tag data.

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

