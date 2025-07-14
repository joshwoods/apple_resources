

- Security
-  SecKeyIsAlgorithmSupported(\_:\_:\_:) 

Function

# SecKeyIsAlgorithmSupported(\_:\_:\_:)

Returns a Boolean indicating whether a key is suitable for an operation using a certain algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyIsAlgorithmSupported(
    _ key: SecKey,
    _ operation: SecKeyOperationType,
    _ algorithm: SecKeyAlgorithm
) -> Bool
```

## Parameters 

`key`  

The key whose suitability you want to test.

`operation`  

The operation that you want to perform with the key. Use one of the values from SecKeyOperationType.

`algorithm`  

The algorithm that you want to perform with the key. Use one of the values from SecKeyAlgorithm.

## Return Value

A Boolean indicating whether the key can be used for the given operation and algorithm.

## Mentioned in 

Signing and Verifying

Using Keys for Encryption

