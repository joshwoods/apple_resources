

- Security
-  AuthorizationFree(\_:\_:) 

Function

# AuthorizationFree(\_:\_:)

Frees the memory associated with an authorization reference.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationFree(
    _ authorization: AuthorizationRef,
    _ flags: AuthorizationFlags
) -> OSStatus
```

## Parameters 

`authorization`  

The authorization reference to free.

`flags`  

A bit mask. In most cases, pass the constant kAuthorizationFlagDefaults. To remove all shared and non-shared authorizations, pass the constant destroyRights.

## Return Value

A result code. See Authorization Services Result Codes.

## Discussion

Call this function when your application no longer needs the authorization reference you created using the function AuthorizationCreate(_:_:_:_:).

