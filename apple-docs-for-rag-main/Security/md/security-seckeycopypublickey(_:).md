

- Security
-  SecKeyCopyPublicKey(\_:) 

Function

# SecKeyCopyPublicKey(\_:)

Gets the public key associated with the given private key.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyCopyPublicKey(_ key: SecKey) -> SecKey?
```

## Parameters 

`key`  

The private key for which you want the corresponding public key.

## Return Value

The public key corresponding to the given private key. In Objective-C, call the CFRelease function to free this key’s memory when you are done with it.

## Mentioned in 

Generating New Cryptographic Keys

Getting an Existing Key

Protecting keys with the Secure Enclave

## Discussion

The returned public key may be `nil` if the app that created the private key didn’t also store the corresponding public key in the keychain, or if the system can’t reconstruct the corresponding public key.

