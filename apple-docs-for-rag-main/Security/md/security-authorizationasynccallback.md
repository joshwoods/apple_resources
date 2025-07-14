

- Security
-  AuthorizationAsyncCallback 

Type Alias

# AuthorizationAsyncCallback

A block used as a callback for the asynchronous version of copying authorization rights.

Mac Catalyst 13.0+macOS 10.7+

``` source
typealias AuthorizationAsyncCallback = (OSStatus, UnsafeMutablePointer?) -> Void
```

## Parameters 

`err`  

A result code. See Authorization Services Result Codes. This is equivalent to the return value from the AuthorizationCopyRights(_:_:_:_:_:) function.

`blockAuthorizedRights`  

The authorized rights. This is equivalent to the authorizedRights parameter of the AuthorizationCopyRights(_:_:_:_:_:) function. Free this object using the AuthorizationFreeItemSet(_:) function when you are done with it.

## Discussion

Use a block of this type as the callback parameter to the AuthorizationCopyRightsAsync(_:_:_:_:_:) function.

