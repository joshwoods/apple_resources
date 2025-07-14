

- Local Authentication
- LAPublicKey
-  canVerify(using:) 

Instance Method

# canVerify(using:)

Checks whether the algorithm you supply is valid for verifying signatures with the key.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func canVerify(using algorithm: SecKeyAlgorithm) -> Bool
```

## Parameters 

`algorithm`  

A cryptographic algorithm.

## Return Value

A Boolean value that indicates whether the algorithm you supply is valid for verifying signatures with the key.

## See Also

### Checking algorithm support

func canEncrypt(using: SecKeyAlgorithm) -> Bool

Checks whether the algorithm you supply is valid for encrypting data with the key.

