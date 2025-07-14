

- Security
-  SecKeyCreateEncryptedData(\_:\_:\_:\_:) 

Function

# SecKeyCreateEncryptedData(\_:\_:\_:\_:)

Encrypts a block of data using a public key and specified algorithm.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func SecKeyCreateEncryptedData(
    _ key: SecKey,
    _ algorithm: SecKeyAlgorithm,
    _ plaintext: CFData,
    _ error: UnsafeMutablePointer?>?
) -> CFData?
```

## Parameters 

`key`  

The public key to use to perform the encryption.

`algorithm`  

The encryption algorithm to use. Use one of the encryption algorithms listed in SecKeyAlgorithm. You can use the SecKeyIsAlgorithmSupported(_:_:_:) function to test that the key is suitable for the algorithm.

`plaintext`  

The data to be encrypted.

`error`  

The address of a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object. If an error occurs, this is set to point at an error instance that describes the failure.

## Return Value

The encrypted data or `NULL` on failure. In Objective-C, call the CFRelease function to free the data’s memory when you are done with it.

## Mentioned in 

Using Keys for Encryption

Generating New Cryptographic Keys

## Discussion

You can decrypt this data with the corresponding private key and a call to SecKeyCreateDecryptedData(_:_:_:_:).

