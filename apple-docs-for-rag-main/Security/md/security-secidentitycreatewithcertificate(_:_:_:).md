

- Security
-  SecIdentityCreateWithCertificate(\_:\_:\_:) 

Function

# SecIdentityCreateWithCertificate(\_:\_:\_:)

Creates a new identity for a certificate and its associated private key.

macOS 10.5+

``` source
func SecIdentityCreateWithCertificate(
    _ keychainOrArray: CFTypeRef?,
    _ certificateRef: SecCertificate,
    _ identityRef: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`keychainOrArray`  

A reference to a keychain or an array of keychains to search for the associated private key. Specify `NULL` to search the user’s default keychain search list.

`certificateRef`  

The certificate for which you want to create an identity.

`identityRef`  

On return, an identity object for the certificate and its associated private key. In Objective-C, call the CFRelease function to release this object when you are finished with it.

## Return Value

A result code. See Security Framework Result Codes.

## Mentioned in 

Creating an Identity

## Discussion

If the associated private key is not found in one of the specified keychains, this function fails with an appropriate error code (usually errSecItemNotFound), and does not return anything in the `identityRef` parameter.

