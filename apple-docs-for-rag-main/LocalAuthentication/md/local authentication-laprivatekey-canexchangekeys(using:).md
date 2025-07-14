

- Local Authentication
- LAPrivateKey
-  canExchangeKeys(using:) 

Instance Method

# canExchangeKeys(using:)

Checks whether the algorithm you supply is valid for performing key exchanges.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func canExchangeKeys(using algorithm: SecKeyAlgorithm) -> Bool
```

## Parameters 

`algorithm`  

A cryptographic algorithm.

## Return Value

A Boolean value that indicates whether the algorithm you supply is valid for performing key exchanges.

## See Also

### Checking algorithm support

func canDecrypt(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for decrypting data with the key.

func canSign(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for signing data with the key.

