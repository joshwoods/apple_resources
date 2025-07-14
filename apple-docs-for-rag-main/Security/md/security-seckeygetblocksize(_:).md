

- Security
-  SecKeyGetBlockSize(\_:) 

Function

# SecKeyGetBlockSize(\_:)

Gets the block length associated with a cryptographic key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 4.0+visionOS 1.0+watchOS 1.0+

``` source
func SecKeyGetBlockSize(_ key: SecKey) -> Int
```

## Parameters 

`key`  

The key for which you want the block length.

## Return Value

The block length associated with the key in bytes. If the key is an RSA key, for example, this is the size of the modulus.

## Mentioned in 

Using Keys for Encryption

