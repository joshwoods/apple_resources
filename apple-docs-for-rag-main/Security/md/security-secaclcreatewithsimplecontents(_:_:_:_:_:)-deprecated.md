

- Security
-  SecACLCreateWithSimpleContents(\_:\_:\_:\_:\_:) Deprecated

Function

# SecACLCreateWithSimpleContents(\_:\_:\_:\_:\_:)

Creates a new ACL entry with the given characteristics, and adds it to an access instance.

macOS 10.7–10.10Deprecated

``` source
func SecACLCreateWithSimpleContents(
    _ access: SecAccess,
    _ applicationList: CFArray?,
    _ description: CFString,
    _ promptSelector: SecKeychainPromptSelector,
    _ newAcl: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`access`  

The access instance to which to add the information.

`applicationList`  

An array of SecTrustedApplication instances identifying apps that are allowed access to the keychain item without user confirmation.

Set this parameter to `nil` to indicate that any app can use this item. Pass an empty array to indicate that there are no trusted apps.

`description`  

The human readable name to be used to refer to this item when the user is prompted.

`promptSelector`  

A set of prompt selector flags. See SecKeychainPromptSelector for possible values.

`newAcl`  

A pointer the method uses to return the new SecACL instance.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The ACL entry returned by this method includes a list of trusted apps, the name of the keychain item as it appears in user prompts, the prompt selector flag, and a list of one or more operations to which this ACL entry applies. By default, a new ACL entry applies to all operations. Use the SecACLUpdateAuthorizations(_:_:) method to set the list of operations for an ACL entry.

Note

Starting in macOS 10.13.1, for added security, the system ignores the `promptSelector` property of an ACL object and always prompts for the keychain password when asking the user whether to add an app to the list of trusted apps.

The system requires exactly one owner ACL entry in each access instance. The SecACLCreateWithSimpleContents(_:_:_:_:_:) method fails if you attempt to add a second owner entry. To change owner access controls, use the SecAccessCopyMatchingACLList(_:_:) function to find the owner entry (the only one with an authorization tag of kSecACLAuthorizationChangeACL) and the SecACLSetContents(_:_:_:_:) method to change it as needed.

