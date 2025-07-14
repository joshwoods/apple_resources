

- Local Authentication
-  LAPublicKey 

Class

# LAPublicKey

The public portion of an asymmetric key pair.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LAPublicKey
```

## Topics

### Checking algorithm support

func canEncrypt(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for encrypting data with the key.

func canVerify(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for verifying signatures with the key.

### Performing cryptographic operations

func encrypt(Data, algorithm: SecKeyAlgorithm, completion: (Data?, (any Error)?) -> Void)

Encrypts the data you supply with a given algorithm.

func exportBytes(completion: (Data?, (any Error)?) -> Void)

Exports the data that represents a public key.

func verify(Data, signature: Data, algorithm: SecKeyAlgorithm, completion: ((any Error)?) -> Void)

Verifies a digital signature for the data you supply.

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

class LAPrivateKey

The private portion of an asymmetric key pair.

