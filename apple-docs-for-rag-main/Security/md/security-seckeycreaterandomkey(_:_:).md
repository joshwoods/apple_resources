

- Security
-  SecKeyCreateRandomKey(\_:\_:) 

Function

# SecKeyCreateRandomKey(\_:\_:)

Generates a new public-private key pair.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyCreateRandomKey(
    _ parameters: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> SecKey?
```

## Parameters 

`parameters`  

A dictionary you use to specify the attributes of the generated keys. See Key Generation Attributes for details.

`error`  

An error reference pointer that SecKeyCreateRandomKey(_:_:) populates with a suitable error instance on failure.

## Return Value

The newly generated private key, or `NULL` on failure. In Objective-C, call the CFRelease function to free the key when you are done with it.

## Mentioned in 

Protecting keys with the Secure Enclave

Generating New Cryptographic Keys

## Discussion

To get the associated public key, use SecKeyCopyPublicKey(_:). SecKeyCreateRandomKey(_:_:) fails and returns errSecInteractionNotAllowed if you call it in the background on iPhone or iPad while the device is locked.

