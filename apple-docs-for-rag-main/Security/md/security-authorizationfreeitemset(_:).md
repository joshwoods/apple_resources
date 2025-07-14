

- Security
-  AuthorizationFreeItemSet(\_:) 

Function

# AuthorizationFreeItemSet(\_:)

Frees the memory associated with a set of authorization items.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationFreeItemSet(_ set: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`set`  

A pointer to the authorization set to free.

## Return Value

A result code. See Authorization Services Result Codes.

## Discussion

When your application no longer needs the authorization item sets created by the Security Server in the AuthorizationCopyRights(_:_:_:_:_:) and AuthorizationCopyInfo(_:_:_:) functions, call this function to free it.

