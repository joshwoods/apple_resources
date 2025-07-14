

- Security
-  SecACLCopyContents(\_:\_:\_:\_:) Deprecated

Function

# SecACLCopyContents(\_:\_:\_:\_:)

Returns the application list, description, and prompt selector for a given ACL entry.

macOS 10.7–10.10Deprecated

``` source
func SecACLCopyContents(
    _ acl: SecACL,
    _ applicationList: UnsafeMutablePointer,
    _ description: UnsafeMutablePointer,
    _ promptSelector: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`acl`  

The ACL entry from which you want information.

`applicationList`  

The address of an array into which a copy of the application list should be stored on return. This array is filled with SecTrustedApplication instances identifying applications that are allowed access to the keychain item without user confirmation.

If the array is `nil`, then any app can use this item. If the array is empty, then there are no trusted applications.

Call the CFRelease method to release this array when you are finished using it.

`description`  

The address of a string into which a copy of the description is stored on return. This description is the name of the keychain item that appears in the dialog box when the user is prompted for permission to use the item.

Note that this name is not necessarily the same as the name displayed for the item by the Keychain Access app.

Call the CFRelease method to release this string when you are finished using it.

`promptSelector`  

The address of a SecKeychainPromptSelector instance into which a copy of the prompt selector is stored on return.

If the requirePassphase bit is set, the user is prompted for the keychain password each time a non-trusted application attempts to access this item, even if the keychain is already unlocked.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

An ACL entry applies to a specific use or set of uses for a specific keychain item. The entry includes a list of trusted applications, the name of the keychain item as it appears in user prompts, the prompt selector flag, and a list of one or more operations to which this ACL entry applies.

Use the SecACLCopyAuthorizations(_:) method to get the list of operations for an ACL entry.

Note

Starting in macOS 10.13.1, for added security, the system ignores the `promptSelector` property of an ACL entry and always prompts for the keychain password when asking the user whether to add an app to the list of trusted apps.

