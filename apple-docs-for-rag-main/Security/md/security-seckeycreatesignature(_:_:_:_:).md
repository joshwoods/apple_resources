

- Security
-  SecKeyCreateSignature(\_:\_:\_:\_:) 

Function

# SecKeyCreateSignature(\_:\_:\_:\_:)

Creates the cryptographic signature for a block of data using a private key and specified algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyCreateSignature(
    _ key: SecKey,
    _ algorithm: SecKeyAlgorithm,
    _ dataToSign: CFData,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

## Parameters 

`key`  

The private key to use in creating the signature.

`algorithm`  

The signing algorithm to use. Use one of the signing algorithms listed in SecKeyAlgorithm. You can use the SecKeyIsAlgorithmSupported(_:_:_:) function to test that the key is suitable for the algorithm.

`dataToSign`  

The data whose signature you want.

`error`  

The address of a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object. If an error occurs, this is set to point at an error instance that describes the failure.

## Return Value

The digital signature or `NULL` on failure. In Objective-C, call the CFRelease function to free the data’s memory when you are done with it.

## Mentioned in 

Signing and Verifying

## Discussion

You later evaluate the combined data and signature with the corresponding public key and a call to the SecKeyVerifySignature(_:_:_:_:_:) function.

