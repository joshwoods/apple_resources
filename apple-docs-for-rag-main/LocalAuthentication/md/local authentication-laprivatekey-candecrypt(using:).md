

- Local Authentication
- LAPrivateKey
-  canDecrypt(using:) 

Instance Method

# canDecrypt(using:)

Checks whether the algorithm you supply is valid for decrypting data with the key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func canDecrypt(using algorithm: SecKeyAlgorithm) -> Bool
```

## Parameters 

`algorithm`  

A cryptographic algorithm.

## Return Value

A Boolean value that indicates whether the algorithm you supply is valid for decrypting data with the key.

## See Also

### Checking algorithm support

func canExchangeKeys(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for performing key exchanges.

func canSign(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for signing data with the key.

