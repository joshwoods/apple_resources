

- Security
-  SecAccessCopyOwnerAndACL(\_:\_:\_:\_:\_:) Deprecated

Function

# SecAccessCopyOwnerAndACL(\_:\_:\_:\_:\_:)

Retrieves the owner and the ACL entries of a given access instance.

macOS 10.7–10.10Deprecated

``` source
func SecAccessCopyOwnerAndACL(
    _ accessRef: SecAccess,
    _ userId: UnsafeMutablePointer?,
    _ groupId: UnsafeMutablePointer?,
    _ ownerType: UnsafeMutablePointer?,
    _ aclList: UnsafeMutablePointer?
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`accessRef`  

An access instance from which to retrieve the owner and ACL entries.

`userId`  

On return, the user ID that owns the access instance.

`groupId`  

On return, the group ID that owns the access instance.

`ownerType`  

On return, flags that indicate whether the specified user ID or group ID owns the resulting ACL entries. See SecAccessOwnerType for details.

`aclList`  

On return, an array of SecACL instances associated with the access instance.

## Return Value

A result code. See Security Framework Result Codes.

