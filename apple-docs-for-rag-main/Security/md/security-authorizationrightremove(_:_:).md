

- Security
-  AuthorizationRightRemove(\_:\_:) 

Function

# AuthorizationRightRemove(\_:\_:)

Removes a right from the policy database.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationRightRemove(
    _ authRef: AuthorizationRef,
    _ rightName: UnsafePointer
) -> OSStatus
```

## Parameters 

`authRef`  

A valid authorization reference used to authorize modifications.

`rightName`  

An ASCII character string representing the right name. This function does not accept wildcard right names.

## Return Value

A result code. See Authorization Services Result Codes.

## Discussion

The right you remove must be an explicit right with no wildcards. Wildcard rights are for use by system administrators for site configuration.

