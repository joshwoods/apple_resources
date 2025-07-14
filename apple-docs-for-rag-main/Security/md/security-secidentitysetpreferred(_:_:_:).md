

- Security
-  SecIdentitySetPreferred(\_:\_:\_:) 

Function

# SecIdentitySetPreferred(\_:\_:\_:)

Sets the identity that should be preferred for the specified name and key use.

macOS 10.7+

``` source
func SecIdentitySetPreferred(
    _ identity: SecIdentity?,
    _ name: CFString,
    _ keyUsage: CFArray?
) -> OSStatus
```

## Parameters 

`identity`  

The identity to set as preferred for the specified name and key usage.

`name`  

A string containing an email address (RFC 822) or other name for which a preferred certificate is requested.

`keyUsage`  

An array containing a list of usage attributes (kSecAttrCanEncrypt, for example), or `NULL` if you want this identity to be preferred for any usage. See Attribute Item Keys for a complete list of possible usage attributes.

## Return Value

A result code. See Security Framework Result Codes.

