

- Security
-  SecAccessCreateWithOwnerAndACL(\_:\_:\_:\_:\_:) Deprecated

Function

# SecAccessCreateWithOwnerAndACL(\_:\_:\_:\_:\_:)

Creates a new access instance using the owner and ACL entries you provide.

macOS 10.7–10.10Deprecated

``` source
func SecAccessCreateWithOwnerAndACL(
    _ userId: uid_t,
    _ groupId: gid_t,
    _ ownerType: SecAccessOwnerType,
    _ acls: CFArray?,
    _ error: UnsafeMutablePointer?>?
) -> SecAccess?
```

Deprecated

SecKeychain is deprecated

## Parameters 

`userId`  

The user ID that owns this ACL.

`groupId`  

The group ID that owns this ACL.

`ownerType`  

Flags that control whether the specified user ID or group ID owns the resulting ACL. See SecAccessOwnerType for details.

`acls`  

An array of ACL entries to associate with the access instance.

`error`  

The address of an error instance. On error, the return value is `nil`, and the variable referenced by this parameter is overwritten with a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 instance that provides more information.

## Return Value

The new access instance. In Objective-C, call the CFRelease function to release it when you are finished using it.

## Discussion

Use this method to create a customized access instance from SecACL instances that you’ve created with the SecACLCreateWithSimpleContents(_:_:_:_:_:) method. If you want a default access instance, use the SecAccessCreate(_:_:_:) method instead.

