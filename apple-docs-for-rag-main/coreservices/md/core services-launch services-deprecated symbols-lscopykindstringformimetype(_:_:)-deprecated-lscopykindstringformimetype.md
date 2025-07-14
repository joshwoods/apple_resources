

- Core Services
- Launch Services
- Deprecated Symbols
-  LSCopyKindStringForMIMEType(\_:\_:) Deprecated

Function

# LSCopyKindStringForMIMEType(\_:\_:)

Obtains the kind string for a specified MIME type.

macOS 10.2–10.10Deprecated

``` source
func LSCopyKindStringForMIMEType(
    _ inMIMEType: CFString!,
    _ outKindString: UnsafeMutablePointer?>!
) -> OSStatus
```

Deprecated

Use UTTypeCopyDescription(_:) instead.

## Parameters 

`inMIMEType`  

A Core Foundation string object specifying the MIME type whose kind string is requested; see the *CFString Reference* in the Core Foundation Reference Documentation for a description of the `CFStringRef` data type. Comparison of MIME types is case-insensitive.

`outKindString`  

A pointer to a Core Foundation string object that, on return, will contain the kind string for the specified MIME type; see the *CFString Reference* in the Core Foundation Reference Documentation for a description of the `CFStringRef` data type. You are responsible for releasing this object.

## Return Value

A result code; see Result Codes.

## Discussion

The kind string (which may be localized) is obtained from the preferred application for opening items of the specified the MIME type, if one is found in the Launch Services database; otherwise, a more generic kind string is chosen.

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

func LSCopyItemAttribute(UnsafePointer&lt;FSRef>!, LSRolesMask, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFTypeRef>?>!) -> OSStatus

Obtains the value of an item’s attribute.

Deprecated

func LSCopyItemAttributes(UnsafePointer&lt;FSRef>!, LSRolesMask, CFArray!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!) -> OSStatus

Obtains multiple item attribute values as a dictionary.

Deprecated

func LSGetExtensionInfo(Int, UnsafePointer&lt;UniChar>!, UnsafeMutablePointer&lt;Int>!) -> OSStatus

Obtains the starting index of the extension within a filename.

Deprecated

func LSSetExtensionHiddenForRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a file-system reference.

Deprecated

func LSSetExtensionHiddenForURL(CFURL!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a URL.

Deprecated

func LSRegisterFSRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Registers an app with a file-system reference in the Launch Services database.

Deprecated

