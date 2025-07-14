

- Security
-  SecPKCS12Import(\_:\_:\_:) 

Function

# SecPKCS12Import(\_:\_:\_:)

Returns the identities and certificates in a PKCS \#12-formatted blob.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func SecPKCS12Import(
    _ pkcs12_data: CFData,
    _ options: CFDictionary,
    _ items: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`pkcs12_data`  

The PKCS \#12 data you wish to decode.

`options`  

A dictionary of key-value pairs specifying options for the function. See Keychain Import and Export Options for a list of valid keys.

`items`  

On return, an array of `CFDictionary` key-value dictionaries. The function returns one dictionary for each item (identity or certificate) in the PKCS \#12 blob. For a list of dictionary keys, see PKCS #12 Import Item Keys.

## Return Value

A result code. See Security Framework Result Codes. The function returns errSecSuccess if there were no errors, errSecDecode if the blob can’t be read or is malformed, and errSecAuthFailed if the password was not correct or data in the blob was damaged.

## Mentioned in 

Importing an Identity

## Discussion

Your application can import a PKCS \#12–formatted blob (a file with extension `.p12`) containing certificates and identities, where an identity is a digital certificate together with its associated private key. You can use the `SecPKCS12Import` function to obtain `SecIdentityRef` objects (including `SecCertificateRef` and `SecKeyRef` objects) for the identities in the blob, together with `SecCertificateRef` objects for the certificates in the blob needed to validate the identity, and `SecTrustRef` trust management objects needed to evaluate trust for the identities. You can then use the Keychain Services API (see Keychain services) to put the identities and associated certificates in the keychain.

