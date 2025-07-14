

- Core Services
- Launch Services
-  LSCopyApplicationURLsForBundleIdentifier(\_:\_:) Deprecated

Function

# LSCopyApplicationURLsForBundleIdentifier(\_:\_:)

Locates all URLs for apps that correspond to the specified bundle identifier.

macOS 10.10–12.0Deprecated

``` source
func LSCopyApplicationURLsForBundleIdentifier(
    _ inBundleIdentifier: CFString,
    _ outError: UnsafeMutablePointer?>?
) -> Unmanaged?
```

## Parameters 

`inBundleIdentifier`  

The bundle identifier of interest, such as "com.apple.finder". Must not be `NULL`.

`outError`  

On failure, set to a `CFError` describing the problem. If you aren't interested in this information, pass `NULL`. The caller is responsible for releasing this object.

## Return Value

The URLs for any applications with the specified bundle identifier returned in a `CFArray`. If no application is found, `NULL` is returned and `outError` (if not `NULL`) is populated with kLSApplicationNotFoundErr.

In macOS 10.15 and later, the returned array is sorted with the first element containing the best available application with the specified bundle identifier. Prior to macOS 10.15, the order of elements in the array was undefined.

The caller is responsible for releasing this array.

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

func LSCanURLAcceptURL(CFURL, CFURL, LSRolesMask, LSAcceptanceFlags, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Tests whether an app can accept (open) an item for a URL.

