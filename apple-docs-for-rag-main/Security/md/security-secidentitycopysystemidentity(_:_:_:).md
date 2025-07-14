

- Security
-  SecIdentityCopySystemIdentity(\_:\_:\_:) 

Function

# SecIdentityCopySystemIdentity(\_:\_:\_:)

Obtains the system identity associated with a specified domain.

macOS 10.5+

``` source
func SecIdentityCopySystemIdentity(
    _ domain: CFString,
    _ idRef: UnsafeMutablePointer,
    _ actualDomain: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`domain`  

The domain for which you want to find an identity, typically in reverse DNS notation, such as `com.apple.security`. You may also pass the values defined in System Identity Domains.

`idRef`  

On return, the identity object of the system-wide identity associated with the specified domain. In Objective-C, call the CFRelease function to release this object when you are finished with it.

`actualDomain`  

On return, the actual domain name of the returned identity object is returned here. This may be different from the requested domain. Pass `NULL` if you do not want this information.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

If no system identity exists for the specified domain, a domain specific alternate may be returned instead. This is typically (but not exclusively) the system default identity. (kSecIdentityDomainDefault).

