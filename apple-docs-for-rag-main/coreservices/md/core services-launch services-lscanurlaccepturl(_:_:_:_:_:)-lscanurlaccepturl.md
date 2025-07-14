

- Core Services
- Launch Services
-  LSCanURLAcceptURL(\_:\_:\_:\_:\_:) 

Function

# LSCanURLAcceptURL(\_:\_:\_:\_:\_:)

Tests whether an app can accept (open) an item for a URL.

macOS 10.0+

``` source
func LSCanURLAcceptURL(
    _ inItemURL: CFURL,
    _ inTargetURL: CFURL,
    _ inRoleMask: LSRolesMask,
    _ inFlags: LSAcceptanceFlags,
    _ outAcceptsItem: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inItemURL`  

A Core Foundation URL reference designating the source item (the item to test for acceptance by the target application); see the *CFURL Reference* in the Core Foundation Reference Documentation for a description of the `CFURLRef` data type.

`inTargetURL`  

A Core Foundation URL reference designating the target application; see the *CFURL Reference* in the Core Foundation Reference Documentation for a description of the `CFURLRef` data type. The URL must have scheme `file` and contain a valid path to an application file or application bundle.

`inRolesMask`  

A bit mask specifying the target app’s desired role or roles with respect to the source item; see LSRolesMask for a description of this mask. This parameter applies only to URLs with a scheme component of `file`, and is ignored for all other schemes. If the role is unimportant, pass `kLSRolesAll`.

`inFlags`  

Flags specifying behavior to observe during the acceptance test; see LSAcceptanceFlags for a description of these flags.

`outAcceptsItem`  

A pointer to a Boolean value that, on return, will indicate whether the target application can accept the source item with at least one of the specified roles.

## Return Value

A result code; see Result Codes.

## Discussion

If the item URL’s scheme is `file` (designating either a file or a directory), the acceptance test is based on the designated item’s filename extension, file type, and creator signature, along with the role specified by the `inRolesMask` parameter; otherwise, it is based on the URL scheme (such as `http`, `ftp`, or `mailto`).

### Version-Notes

Thread-safe since Mac OS version 10.2.

## See Also

### Locating an App

func LSCopyDefaultApplicationURLForURL(CFURL, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens an item.

Deprecated

func LSCopyDefaultApplicationURLForContentType(CFString, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens a content type.

Deprecated

func LSCopyApplicationURLsForURL(CFURL, LSRolesMask) -> Unmanaged&lt;CFArray>?

Locates all known apps suitable for opening an item for the specified URL.

Deprecated

func LSCopyApplicationURLsForBundleIdentifier(CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFArray>?

Locates all URLs for apps that correspond to the specified bundle identifier.

Deprecated

