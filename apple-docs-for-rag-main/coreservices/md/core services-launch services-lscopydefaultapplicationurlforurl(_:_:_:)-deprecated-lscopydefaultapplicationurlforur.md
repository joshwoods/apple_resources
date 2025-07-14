

- Core Services
- Launch Services
-  LSCopyDefaultApplicationURLForURL(\_:\_:\_:) Deprecated

Function

# LSCopyDefaultApplicationURLForURL(\_:\_:\_:)

Returns the app that opens an item.

macOS 10.10–12.0Deprecated

``` source
func LSCopyDefaultApplicationURLForURL(
    _ inURL: CFURL,
    _ inRoleMask: LSRolesMask,
    _ outError: UnsafeMutablePointer?>?
) -> Unmanaged?
```

## Parameters 

`inURL`  

The URL of the item for which the app is requested.

`inRoleMask`  

Whether to return the editor or viewer for `inURL`. If you don't care which, use all.

`outError`  

On failure, set to a CFError describing the problem. If you are not interested in this information, pass `NULL`. The caller is responsible for releasing this object.

## Return Value

If an acceptable app is found, its URL is returned. If the URL is a `file://` URL, the application bound to the specified file or directory's type is returned. If the URL's scheme is something else, its default scheme handler is returned. If no app could be found, `NULL` is returned and outError (if not `NULL`) is populated with kLSApplicationNotFoundErr. The caller is responsible for releasing this URL.

## Discussion

Consults the binding tables to return the application that would be used to open inURL if it were double-clicked in the Finder. This application will be the user-specified override if appropriate or the default otherwise.

## See Also

### Locating an App

func LSCopyDefaultApplicationURLForContentType(CFString, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens a content type.

Deprecated

func LSCopyApplicationURLsForURL(CFURL, LSRolesMask) -> Unmanaged&lt;CFArray>?

Locates all known apps suitable for opening an item for the specified URL.

Deprecated

func LSCanURLAcceptURL(CFURL, CFURL, LSRolesMask, LSAcceptanceFlags, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Tests whether an app can accept (open) an item for a URL.

func LSCopyApplicationURLsForBundleIdentifier(CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFArray>?

Locates all URLs for apps that correspond to the specified bundle identifier.

Deprecated

