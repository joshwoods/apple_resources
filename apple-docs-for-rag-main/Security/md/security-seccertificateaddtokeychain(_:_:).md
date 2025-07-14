

- Security
-  SecCertificateAddToKeychain(\_:\_:) 

Function

# SecCertificateAddToKeychain(\_:\_:)

Adds a certificate to a keychain.

macOS 10.3+

``` source
func SecCertificateAddToKeychain(
    _ certificate: SecCertificate,
    _ keychain: SecKeychain?
) -> OSStatus
```

## Parameters 

`certificate`  

The certificate object for the certificate to add to the keychain.

`keychain`  

The keychain object for the keychain to which you want to add the certificate. Pass `NULL` to add the certificate to the default keychain.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Important

To add a certificate to the login keychain, use SecItemAdd(_:_:) instead.

This function requires a certificate object, which can, for example, be created with the SecCertificateCreateFromData function or obtained over a network (see Secure Transport). If the certificate has already been added to the specified keychain, the function returns errSecDuplicateItem and does not add another copy to the keychain. The function looks at the certificate data, not at the certificate object, to determine whether the certificate is a duplicate. It considers two certificates to be duplicates if they have the same primary key attributes.

### Special Considerations

If the keychain is locked, the system asks the user for a password or other token to unlock it. This function can therefore block while waiting for user input.

