

- Security
-  SecKeyCreateDecryptedData(\_:\_:\_:\_:) 

Function

# SecKeyCreateDecryptedData(\_:\_:\_:\_:)

Decrypts a block of data using a private key and specified algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyCreateDecryptedData(
    _ key: SecKey,
    _ algorithm: SecKeyAlgorithm,
    _ ciphertext: CFData,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

## Parameters 

`key`  

The private key to use to perform the decryption.

`algorithm`  

The algorithm that was used to encrypt the data in the first place. Use one of the encryption algorithms listed in SecKeyAlgorithm. You can use the SecKeyIsAlgorithmSupported(_:_:_:) function to test that the key is suitable for the algorithm.

`ciphertext`  

The data, produced with the corresponding public key and a call to the SecKeyCreateEncryptedData(_:_:_:_:) function, that you want to decrypt.

`error`  

The address of a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object. If an error occurs, this is set to point at an error instance that describes the failure.

## Return Value

The decrypted data or `NULL` on failure. In Objective-C, call the CFRelease function to free the data’s memory when you are done with it.

## Mentioned in 

Using Keys for Encryption

Generating New Cryptographic Keys

