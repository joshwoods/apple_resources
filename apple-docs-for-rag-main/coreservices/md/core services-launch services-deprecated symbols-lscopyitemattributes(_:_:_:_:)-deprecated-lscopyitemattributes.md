

- Core Services
- Launch Services
- Deprecated Symbols
-  LSCopyItemAttributes(\_:\_:\_:\_:) Deprecated

Function

# LSCopyItemAttributes(\_:\_:\_:\_:)

Obtains multiple item attribute values as a dictionary.

macOS 10.4–10.10Deprecated

``` source
func LSCopyItemAttributes(
    _ inItem: UnsafePointer!,
    _ inRoles: LSRolesMask,
    _ inAttributeNames: CFArray!,
    _ outValues: UnsafeMutablePointer?>!
) -> OSStatus
```

Deprecated

Use CFURLCopyResourcePropertiesForKeys(_:_:_:) or resourceValues(forKeys:) instead.

## Parameters 

`inItem`  

The `FSRef` of the item to query.

`inRoles`  

The roles. When obtaining attributes related to document binding (such as `kLSItemRoleHandlerDisplayName`), at least one of the roles must be provided by the application selected. Pass `kLSRolesAll` if any role is acceptable.

`inAttributeNames`  

A `CFArrayRef` for an array containing the attribute names to copy. For possible values, see `Item Attribute Constants`.

`outValues`  

On return, a pointer a `CFDictionaryRef` for a dictionary whose keys are the attribute names specified by the `inAttributeNames` parameter and whose values are the attribute’s values. The `CFTypeID` of each value in the dictionary varies by attribute. See `Item Attribute Constants` for the data type of each value. If the item does not have a specified attribute, the key for the attribute is not in the dictionary.

## Return Value

A result code; see Result Codes.

## Discussion

Thread-safe since OS X v10.4.

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

