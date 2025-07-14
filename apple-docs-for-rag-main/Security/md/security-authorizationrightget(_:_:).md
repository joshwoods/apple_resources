

- Security
-  AuthorizationRightGet(\_:\_:) 

Function

# AuthorizationRightGet(\_:\_:)

Retrieves a right definition as a dictionary.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationRightGet(
    _ rightName: UnsafePointer,
    _ rightDefinition: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`rightName`  

An ASCII character string representing the right name. Wildcard right names are valid.

`rightDefinition`  

A reference to a dictionary. On return, this points to a dictionary of keys that define the right. Passing `nil` checks if the right is defined. You should release the memory used by the returned dictionary.

## Return Value

A result code. See Authorization Services Result Codes.

## Discussion

You do not need an authorization reference to use this function because the policy database is world readable.

