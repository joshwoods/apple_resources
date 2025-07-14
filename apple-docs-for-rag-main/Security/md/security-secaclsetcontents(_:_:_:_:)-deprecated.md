

- Security
-  SecACLSetContents(\_:\_:\_:\_:) Deprecated

Function

# SecACLSetContents(\_:\_:\_:\_:)

Sets the application list, description, and prompt selector for a given ACL entry.

macOS 10.7–10.10Deprecated

``` source
func SecACLSetContents(
    _ acl: SecACL,
    _ applicationList: CFArray?,
    _ description: CFString,
    _ promptSelector: SecKeychainPromptSelector
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`acl`  

The ACL entry to modify.

`applicationList`  

An array of SecTrustedApplication instances identifying apps that are allowed access to the keychain item without user confirmation. Use the SecTrustedApplicationCreateFromPath(_:_:) method to create trusted app objects.

If you set this parameter to `nil`, then any app can use this item. If you pass an empty array, then no apps are trusted.

`description`  

The name of the keychain item that appears in the dialog box when the user is prompted for permission to use the item. Note that this name is not necessarily the same as the one displayed for the item by the Keychain Access app.

`promptSelector`  

The prompt selector flags for the given access control list entry. See SecKeychainPromptSelector for details.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Because an ACL entry is always associated with an access instance, when you modify the entry, you are modifying the access instance as well.

Use the SecACLCopyAuthorizations(_:) method to get the list of operations for an ACL entry.

Note

Starting in macOS 10.13.1, for added security, the system ignores the `promptSelector` property of an ACL entry and always prompts for the keychain password when asking the user whether to add an app to the list of trusted apps.

