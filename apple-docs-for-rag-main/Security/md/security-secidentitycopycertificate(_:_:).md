

- Security
-  SecIdentityCopyCertificate(\_:\_:) 

Function

# SecIdentityCopyCertificate(\_:\_:)

Retrieves a certificate associated with an identity.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecIdentityCopyCertificate(
    _ identityRef: SecIdentity,
    _ certificateRef: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`identityRef`  

The identity object for the identity whose certificate you wish to retrieve.

`certificateRef`  

On return, points to the certificate object associated with the specified identity. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Parsing an Identity

## Discussion

An identity is a digital certificate together with its associated private key.

For a certificate in a keychain, you can cast the `SecCertificateRef` data type to a `SecKeychainItemRef` for use with Keychain Services functions.

