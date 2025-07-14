

- Security
-  SecCertificateCopyPreferred(\_:\_:) 

Function

# SecCertificateCopyPreferred(\_:\_:)

Returns the preferred certificate for the specified name and key usage.

macOS 10.7+

``` source
func SecCertificateCopyPreferred(
    _ name: CFString,
    _ keyUsage: CFArray?
) -> SecCertificate?
```

## Parameters 

`name`  

A string containing an email address (RFC 822) or other name for which a preferred certificate is requested.

`keyUsage`  

An array containing a list of usage attributes (kSecAttrCanEncrypt, for example), or `NULL` if you do not want to request a certificate based on a particular usage. See Attribute Item Keys for a complete list of possible usage attributes.

## Return Value

The preferred certificate for the specified name and key usage, or `NULL` if a matching certificate does not exist. In Objective-C, free the certificate with a call to the CFRelease function when you are done with it.

## Discussion

This function is typically used to obtain the preferred encryption certificate for an email recipient. If a preferred certificate has not been set for the supplied name, this function returns `NULL`. Your code should then perform a search for possible certificates by calling SecItemCopyMatching(_:_:).

