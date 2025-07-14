

- Security
-  SecACLUpdateAuthorizations(\_:\_:) Deprecated

Function

# SecACLUpdateAuthorizations(\_:\_:)

Sets the authorization tags for a given ACL.

macOS 10.7–10.10Deprecated

``` source
func SecACLUpdateAuthorizations(
    _ acl: SecACL,
    _ authorizations: CFArray
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`acl`  

An ACL object that identifies the access control list entry for which you wish to set authorization tags.

`authorizations`  

An array of authorization tags. See `CSSM_ACL_AUTHORIZATION_TAG` for details.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

An ACL entry includes a list of trusted apps, the name of the keychain item as it appears in user prompts, the prompt selector flag, and a list of one or more operations to which this ACL entry applies. Use this method to set a list of operations for an ACL entry, or set the kSecACLAuthorizationAny tag to allow all operations. Use the SecACLSetContents(_:_:_:_:) method to set the other information.

Because an ACL entry is always associated with an access instance, when you modify an entry, you are modifying the access instance as well.

