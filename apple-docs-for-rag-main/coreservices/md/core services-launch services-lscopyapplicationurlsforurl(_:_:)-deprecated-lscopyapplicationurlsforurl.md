

- Core Services
- Launch Services
-  LSCopyApplicationURLsForURL(\_:\_:) Deprecated

Function

# LSCopyApplicationURLsForURL(\_:\_:)

Locates all known apps suitable for opening an item for the specified URL.

macOS 10.3–12.0Deprecated

``` source
func LSCopyApplicationURLsForURL(
    _ inURL: CFURL,
    _ inRoleMask: LSRolesMask
) -> Unmanaged?
```

## Parameters 

`inURL`  

A Core Foundation URL reference designating the item for which all suitable apps are requested. See `CFURL` for a description of the `CFURLRef` data type.

`inRolesMask`  

A bit mask specifying the apps’ role or roles with respect to the designated item. See LSRolesMask for a description of this mask. This parameter applies only to URLs with a scheme component of `file`, and is ignored for all other schemes. If the role is unimportant, pass `kLSRolesAll`.

## Return Value

An array of Core Foundation URL references, one for each app that can open the designated item with at least one of the specified roles. You are responsible for releasing the array object. If no suitable apps are found in the Launch Services database, the function will return `NULL.`

In macOS 10.15 and later, the returned array is sorted with the first element containing the best available apps for opening the specified URL. Prior to macOS 10.15, the order of elements in the array was undefined.

## Discussion

If the item URL’s scheme is `file` (designating either a file or a directory), the selection of suitable applications is based on the designated item’s filename extension, file type, and creator signature, along with the role specified by the `inRolesMask` parameter. Otherwise, the selection is based on the URL scheme (such as `http`, `ftp`, or `mailto`).

### Version Notes

Thread-safe since macOS 10.3.

## See Also

### Locating an App

func LSCopyDefaultApplicationURLForURL(CFURL, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens an item.

Deprecated

func LSCopyDefaultApplicationURLForContentType(CFString, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens a content type.

Deprecated

func LSCanURLAcceptURL(CFURL, CFURL, LSRolesMask, LSAcceptanceFlags, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Tests whether an app can accept (open) an item for a URL.

func LSCopyApplicationURLsForBundleIdentifier(CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFArray>?

Locates all URLs for apps that correspond to the specified bundle identifier.

Deprecated

