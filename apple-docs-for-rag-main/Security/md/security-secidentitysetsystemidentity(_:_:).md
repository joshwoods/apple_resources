

- Security
-  SecIdentitySetSystemIdentity(\_:\_:) 

Function

# SecIdentitySetSystemIdentity(\_:\_:)

Assigns the system identity to be associated with a specified domain.

macOS 10.5+

``` source
func SecIdentitySetSystemIdentity(
    _ domain: CFString,
    _ idRef: SecIdentity?
) -> OSStatus
```

## Parameters 

`domain`  

The domain to which the specified identity will be assigned, typically in reverse DNS notation, such as `com.apple.security`. You may also pass the values defined in System Identity Domains.

`idRef`  

The identity to be assigned to the specified domain. Pass `NULL` to delete any currently-assigned identity for the specified domain; in this case, it is not an error if no identity exists for the specified domain.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The caller must be running as root.

