

- CryptoTokenKit
- TKTokenKeyAlgorithm
-  supportsAlgorithm(\_:) 

Instance Method

# supportsAlgorithm(\_:)

Whether the specified algorithm is the target operation algorithm, or one of the other algorithms used.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func supportsAlgorithm(_ algorithm: SecKeyAlgorithm) -> Bool
```

## Parameters 

`algorithm`  

The algorithm to be checked.

## Return Value

true if `algorithm` is the target operation algorithm or one of the other algorithms used; otherwise, false.

## See Also

### Determining Algorithm Usage

func isAlgorithm(SecKeyAlgorithm) -> Bool

Returns whether the specified algorithm is the target operation algorithm.

