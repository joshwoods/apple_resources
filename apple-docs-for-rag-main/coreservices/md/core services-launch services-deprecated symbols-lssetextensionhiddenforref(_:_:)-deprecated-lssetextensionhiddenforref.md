

- Core Services
- Launch Services
- Deprecated Symbols
-  LSSetExtensionHiddenForRef(\_:\_:) Deprecated

Function

# LSSetExtensionHiddenForRef(\_:\_:)

Specifies whether to show or hide the filename extension for an item with a file-system reference.

macOS 10.1–10.10Deprecated

``` source
func LSSetExtensionHiddenForRef(
    _ inRef: UnsafePointer!,
    _ inHide: Bool
) -> OSStatus
```

Deprecated

Use LSSetExtensionHiddenForURL(_:_:) or the URL resource property kCFURLHasHiddenExtensionKey/hasHiddenExtensionKey instead.

## Parameters 

`inRef`  

A pointer to a file-system reference designating the item whose filename extension is to be hidden or shown; see the *File Manager Reference* in the Carbon File Management Documentation for a description of the `FSRef` data type.

`inHide`  

A Boolean value specifying whether the filename extension should be hidden (`true`) or shown (`false`).

## Return Value

A result code; see Result Codes. The function will return the result code `kLSCannotSetInfoErr` if:

- The extension is not valid (contains spaces)

- The extension is not active (is not claimed by an application registered with Launch Services)

- Hiding the extension would make the filename appear to have an active but incorrect extension (for example, in the filename `Photo.jpeg.scpt`, where hiding the extension would make an AppleScript file appear to be a JPEG file)

## Discussion

This function sets the necessary file-system state controlling whether the filename extension should be hidden in the display name of the item designated by the `inRef` parameter. To determine whether an item’s extension is currently hidden, you can use the `LSCopyItemInfoForRef` function.

### Version-Notes

Thread-safe since Mac OS version 10.2.

## See Also

### Deprecated Functions

func LSGetHandlerOptionsForContentType(CFString!) -> LSHandlerOptions

Gets the handler options for the specified content type.

Deprecated

func LSSetHandlerOptionsForContentType(CFString!, LSHandlerOptions) -> OSStatus

Sets the handler option for the specified content type.

Deprecated

func LSCopyAllHandlersForURLScheme(CFString) -> Unmanaged&lt;CFArray>?

Locates app bundle identifiers for apps capable of handling the specified URL scheme.

Deprecated

func LSCopyDefaultHandlerForURLScheme(CFString) -> Unmanaged&lt;CFString>?

Returns the bundle identifier of the user’s preferred default handler for the specified URL scheme.

Deprecated

func LSGetApplicationForItem(UnsafePointer&lt;FSRef>!, LSRolesMask, UnsafeMutablePointer&lt;FSRef>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!) -> OSStatus

Locates the preferred app for opening an item with a file-system reference.

Deprecated

func LSGetApplicationForURL(CFURL!, LSRolesMask, UnsafeMutablePointer&lt;FSRef>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!) -> OSStatus

Locates the preferred app for opening an item with a URL.

Deprecated

func LSGetApplicationForInfo(OSType, OSType, CFString!, LSRolesMask, UnsafeMutablePointer&lt;FSRef>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!) -> OSStatus

Locates the preferred app for opening items with a specified file type, creator signature, filename extension, or any combination of these characteristics.

Deprecated

func LSCopyApplicationForMIMEType(CFString!, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!) -> OSStatus

Locates the preferred app for opening items with a specified MIME type.

Deprecated

func LSCanRefAcceptItem(UnsafePointer&lt;FSRef>!, UnsafePointer&lt;FSRef>!, LSRolesMask, LSAcceptanceFlags, UnsafeMutablePointer&lt;DarwinBoolean>!) -> OSStatus

Tests whether an app can accept (open) an item with a file-system reference.

Deprecated

func LSFindApplicationForInfo(OSType, CFString!, CFString!, UnsafeMutablePointer&lt;FSRef>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!) -> OSStatus

Locates an app with a specified creator signature, bundle ID, filename, or any combination of these characteristics.

Deprecated

func LSOpenApplication(UnsafePointer&lt;LSApplicationParameters>!, UnsafeMutablePointer&lt;ProcessSerialNumber>!) -> OSStatus

Launches the specified app.

Deprecated

func LSOpenItemsWithRole(UnsafePointer&lt;FSRef>!, CFIndex, LSRolesMask, UnsafePointer&lt;AEKeyDesc>!, UnsafePointer&lt;LSApplicationParameters>!, UnsafeMutablePointer&lt;ProcessSerialNumber>!, CFIndex) -> OSStatus

Opens items with an array of file-system references with a specified role.

Deprecated

func LSOpenURLsWithRole(CFArray!, LSRolesMask, UnsafePointer&lt;AEKeyDesc>!, UnsafePointer&lt;LSApplicationParameters>!, UnsafeMutablePointer&lt;ProcessSerialNumber>!, CFIndex) -> OSStatus

Opens one or more URLs with the specified roles.

Deprecated

func LSOpenFSRef(UnsafePointer&lt;FSRef>!, UnsafeMutablePointer&lt;FSRef>!) -> OSStatus

Opens an item with a file-system reference in the default manner in its preferred app.

Deprecated

func LSOpenFromRefSpec(UnsafePointer&lt;LSLaunchFSRefSpec>!, UnsafeMutablePointer&lt;FSRef>!) -> OSStatus

Opens one or more items with a file-system reference in either their preferred apps or a designated app.

Deprecated

func LSCopyItemInfoForRef(UnsafePointer&lt;FSRef>!, LSRequestedInfo, UnsafeMutablePointer&lt;LSItemInfoRecord>!) -> OSStatus

Obtains requested information about an item with a file-system reference.

Deprecated

func LSCopyItemInfoForURL(CFURL!, LSRequestedInfo, UnsafeMutablePointer&lt;LSItemInfoRecord>!) -> OSStatus

Obtains requested information about an item with a URL.

Deprecated

func LSCopyDisplayNameForRef(UnsafePointer&lt;FSRef>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

Obtains the display name for an item with a file-system reference.

Deprecated

func LSCopyDisplayNameForURL(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

Obtains the display name for an item with a URL.

Deprecated

func LSCopyKindStringForRef(UnsafePointer&lt;FSRef>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

Obtains the kind string for an item with a file-system reference.

Deprecated

func LSCopyKindStringForURL(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

Obtains the kind string for an item with a URL.

Deprecated

func LSCopyKindStringForTypeInfo(OSType, OSType, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

Obtains a kind string for items with a specified file type, creator signature, filename extension, or any combination of these characteristics.

Deprecated

func LSCopyKindStringForMIMEType(CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

Obtains the kind string for a specified MIME type.

Deprecated

func LSCopyItemAttribute(UnsafePointer&lt;FSRef>!, LSRolesMask, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>!) -> OSStatus

Obtains the value of an item’s attribute.

Deprecated

func LSCopyItemAttributes(UnsafePointer&lt;FSRef>!, LSRolesMask, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!) -> OSStatus

Obtains multiple item attribute values as a dictionary.

Deprecated

func LSGetExtensionInfo(Int, UnsafePointer&lt;UniChar>!, UnsafeMutablePointer&lt;Int>!) -> OSStatus

Obtains the starting index of the extension within a filename.

Deprecated

func LSSetExtensionHiddenForURL(CFURL!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a URL.

Deprecated

func LSRegisterFSRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Registers an app with a file-system reference in the Launch Services database.

Deprecated

