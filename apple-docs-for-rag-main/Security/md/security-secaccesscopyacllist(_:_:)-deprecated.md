

- Security
-  SecAccessCopyACLList(\_:\_:) Deprecated

Function

# SecAccessCopyACLList(\_:\_:)

Retrieves all the ACL entries of a given access instance.

macOS 10.2–10.10Deprecated

``` source
func SecAccessCopyACLList(
    _ accessRef: SecAccess,
    _ aclList: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`accessRef`  

The access instance from which to retrieve the information.

`aclList`  

A pointer the method uses to return an array of SecACL instances. In Objective-C, call the CFRelease function to release the array when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

An access instance can have any number of ACL entries for specific operations or sets of operations. Use this method to get an array of all the ACL entries of a particular access instance. To retrieve entries corresponding to specific operations, use the SecAccessCopyMatchingACLList(_:_:) method instead.

