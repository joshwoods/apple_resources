

- Security
-  AuthorizationCreateFromExternalForm(\_:\_:) 

Function

# AuthorizationCreateFromExternalForm(\_:\_:)

Internalizes the external representation of an authorization reference.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationCreateFromExternalForm(
    _ extForm: UnsafePointer,
    _ authorization: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`extForm`  

A pointer to the external representation of the authorization reference you retrieve from the calling process.

`authorization`  

A pointer to an authorization reference. On return, this points to the local copy of the authorization reference. The Security Server allocates the authorization reference for you, so you do not need to call the function AuthorizationCreate(_:_:_:_:).

## Return Value

A result code. See Authorization Services Result Codes.

## Discussion

When passing an authorization reference between processes, use this function to internalize the external representation of the authorization reference you created using the function AuthorizationMakeExternalForm(_:_:).

