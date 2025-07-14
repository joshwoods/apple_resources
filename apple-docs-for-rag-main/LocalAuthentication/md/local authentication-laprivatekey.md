

- Local Authentication
-  LAPrivateKey 

Class

# LAPrivateKey

The private portion of an asymmetric key pair.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LAPrivateKey
```

## Topics

### Accessing the associated public key

var publicKey: LAPublicKey

The public key that corresponds with the private key in a key pair.

### Checking algorithm support

func canDecrypt(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for decrypting data with the key.

func canExchangeKeys(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for performing key exchanges.

func canSign(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for signing data with the key.

### Performing cryptographic operations

func decrypt(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Decrypts the data you supply with a given algorithm.

func exchangeKeys(publicKey: Data, algorithm: SecKeyAlgorithm, parameters: [AnyHashable : Any], completion: (Data?, (any Error)?) -> Void)

Performs a Diffie-Hellman style key exchange operation.

func sign(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Generates a digital signature for the data you supply.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Key pairs

class LAPublicKey

The public portion of an asymmetric key pair.

