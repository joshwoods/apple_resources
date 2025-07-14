

- Security
-  AuthorizationCopyInfo(\_:\_:\_:) 

Function

# AuthorizationCopyInfo(\_:\_:\_:)

Retrieves supporting data such as the user name and other information gathered during evaluation of authorization.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationCopyInfo(
    _ authorization: AuthorizationRef,
    _ tag: AuthorizationString?,
    _ info: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`authorization`  

An authorization reference referring to the authorization session.

`tag`  

An AuthorizationString specifying the type of data the Security Server should return. Pass `nil` to retrieve all available information.

`info`  

A pointer to an authorization set the Security Server creates. On return, this set contains side-band authorization data. When this set is no longer needed, free the memory associated with it by calling the function AuthorizationFreeItemSet(_:).

## Return Value

A result code. See Authorization Services Result Codes.

## Mentioned in 

Extending authorization services with plug-ins

## Discussion

An authorization plug-in can store the results of an authentication operation by calling the SetContextValue function. You can use the AuthorizationCopyInfo(_:_:_:) function to retrieve this information.

