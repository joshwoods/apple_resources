

- Local Authentication
- LAPrivateKey
-  canSign(using:) 

Instance Method

# canSign(using:)

Checks whether the algorithm you supply is valid for signing data with the key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func canSign(using algorithm: SecKeyAlgorithm) -> Bool
```

## Parameters 

`algorithm`  

A cryptographic algorithm.

## Return Value

A Boolean value that indicates whether the algorithm you supply is valid for signing data with the key.

## See Also

### Checking algorithm support

func canDecrypt(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for decrypting data with the key.

func canExchangeKeys(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for performing key exchanges.

