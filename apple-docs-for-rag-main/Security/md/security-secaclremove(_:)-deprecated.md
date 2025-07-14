

- Security
-  SecACLRemove(\_:) Deprecated

Function

# SecACLRemove(\_:)

Removes the specified ACL entry from the access instance that contains it.

macOS 10.3–10.10Deprecated

``` source
func SecACLRemove(_ aclRef: SecACL) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`aclRef`  

An ACL entry to remove.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This method fails if you attempt to remove the owner entry because an access instance must have exactly one such ACL at all times. If you need to change ownership settings, modify the existing owner entry rather than replacing it. In particular, use the SecAccessCopyMatchingACLList(_:_:) method with the kSecACLAuthorizationChangeACL authorization to find the existing entry, and the SecACLSetContents(_:_:_:_:) method to change it as needed.

