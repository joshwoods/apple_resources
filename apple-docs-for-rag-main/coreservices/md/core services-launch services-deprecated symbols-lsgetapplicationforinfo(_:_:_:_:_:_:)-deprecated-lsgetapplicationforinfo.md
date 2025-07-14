

- Core Services
- Launch Services
- Deprecated Symbols
-  LSGetApplicationForInfo(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# LSGetApplicationForInfo(\_:\_:\_:\_:\_:\_:)

Locates the preferred app for opening items with a specified file type, creator signature, filename extension, or any combination of these characteristics.

macOS 10.0–10.10Deprecated

``` source
func LSGetApplicationForInfo(
    _ inType: OSType,
    _ inCreator: OSType,
    _ inExtension: CFString!,
    _ inRoleMask: LSRolesMask,
    _ outAppRef: UnsafeMutablePointer!,
    _ outAppURL: UnsafeMutablePointer?>!
) -> OSStatus
```

Deprecated

Use LSCopyDefaultApplicationURLForContentType(_:_:_:) instead.

## Parameters 

`inType`  

The file type to consider. Comparison of file types is case-sensitive. Pass `kLSUnknownType` if the items’ file type is unimportant.

`inCreator`  

The creator signature to consider. Comparison of creator signatures is case-sensitive. Pass `kLSUnknownCreator` if the items’ creator signature is unimportant.

Note

In macOS 10.6 and later, the `inCreator` parameter is ignored.

`inExtension`  

A Core Foundation string object specifying the filename extension to consider; see the *CFString Reference* in the Core Foundation Reference Documentation for a description of the `CFStringRef` data type. Comparison of filename extensions is case-insensitive. Pass `NULL` if the items’ filename extension is unimportant.

`inRolesMask`  

A bit mask specifying the application’s desired role or roles with respect to items with the specified characteristics; see LSRolesMask for a description of this mask. If the role is unimportant, pass `kLSRolesAll`.

`outAppRef`  

A pointer to a file-system reference that, on return, will identify the preferred application for opening items with the specified characteristics; see the *File Manager Reference* in the Carbon File Management Documentation for a description of the `FSRef` data type. Pass `NULL` if you are not interested in identifying the preferred application in this form; however, this parameter and `outAppURL` cannot both be `NULL`.

`outAppURL`  

A pointer to a Core Foundation URL reference that, on return, will identify the preferred application for items with the specified characteristics; see the *CFURL Reference* in the Core Foundation Reference Documentation for a description of the `CFURLRef` data type. Pass `NULL` if you are not interested in identifying the preferred application in this form; however, this parameter and `outAppRef` cannot both be `NULL`.

Despite the absence of the word `Copy` in its name, this function retains the URL reference object on your behalf; you are responsible for releasing this object.

## Return Value

A result code; see Result Codes. If no application suitable for opening items with the specified characteristics is found in the Launch Services database, the function will return the result code `kLSApplicationNotFoundErr`.

## Discussion

You can request any combination of one, two, or all three of the characteristics specified by the `inType`, `inCreator`, and `inExtension` parameters; at least one of these characteristics must be supplied. Note that since the choice of a preferred application is subject to any document binding preferences the user may have set, the application chosen will not necessarily be the default application that matches the input characteristics, but may instead be a user-specified application that overrides the default.

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

func LSSetExtensionHiddenForRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a file-system reference.

Deprecated

func LSSetExtensionHiddenForURL(CFURL!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a URL.

Deprecated

func LSRegisterFSRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Registers an app with a file-system reference in the Launch Services database.

Deprecated

