

- Core Services
- Launch Services
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Apple has deprecated these symbols and no longer recommends using them.

## Topics

### Deprecated Constants

let kLSItemContentType: CFString!

The item’s content type identifier, which is a uniform type identifier string.

Deprecated

let kLSItemFileType: CFString!

The item’s file type.

Deprecated

let kLSItemFileCreator: CFString!

The item’s file creator.

Deprecated

let kLSItemExtension: CFString!

The item’s filename extension.

Deprecated

let kLSItemDisplayName: CFString!

The item’s name to display to the user. The display name reflects localization and extension hiding that may be in effect.

Deprecated

let kLSItemDisplayKind: CFString!

The localized kind string that describes the item’s type.

Deprecated

let kLSItemRoleHandlerDisplayName: CFString!

The display name of the application that is set to handle this item, subject to the role mask.

Deprecated

let kLSItemIsInvisible: CFString!

A Boolean value that indicates the item is hidden from users.

Deprecated

let kLSItemExtensionIsHidden: CFString!

A Boolean value that indicates the item’s extension is hidden.

Deprecated

### Deprecated Structures

struct LSApplicationParameters

The specification that defines the app, launch flags, and additional parameters that control how an app launches.

Deprecated

struct LSLaunchFSRefSpec

The specification that defines, by file-system reference, an app to launch, items to open, or both, along with related information.

Deprecated

struct LSItemInfoRecord

The specification that contains requested information about an item.

Deprecated

### Deprecated Variables

var kLSLaunchHasUntrustedContents: Int

A request that the system marks the launch items as untrustworthy.

Deprecated

var kLSLaunchNoParams: Int

A request that the system uses the app’s information property to determine the launch parameters.

Deprecated

var kLSLaunchInhibitBGOnly: Int

A request that the system fails the launch if the app is background-only.

Deprecated

var kLSLaunchInClassic: Int

A request that the system forces the app to launch in the Classic emulation environment.

Deprecated

var kLSLaunchStartClassic: Int

A request that the system starts up the Classic emulation environment if the app requires it. If this flag is not set and the app requires the Classic environment, the launch fails.

Deprecated

let kLSItemQuarantineProperties: CFString!Deprecated

var kLSSharedFileListFavoriteItems: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListFavoriteVolumes: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListItemBeforeFirst: Unmanaged&lt;LSSharedFileListItem>Deprecated

var kLSSharedFileListItemHidden: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListItemLast: Unmanaged&lt;LSSharedFileListItem>Deprecated

var kLSSharedFileListLoginItemHidden: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListRecentApplicationItems: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListRecentDocumentItems: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListRecentItemsMaxAmount: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListRecentServerItems: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListSessionLoginItems: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListVolumesComputerVisible: Unmanaged&lt;CFString>Deprecated

var kLSSharedFileListVolumesNetworkVisible: Unmanaged&lt;CFString>Deprecated

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

func LSSetExtensionHiddenForRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a file-system reference.

Deprecated

func LSSetExtensionHiddenForURL(CFURL!, Bool) -> OSStatus

Specifies whether to show or hide the filename extension for an item with a URL.

Deprecated

func LSRegisterFSRef(UnsafePointer&lt;FSRef>!, Bool) -> OSStatus

Registers an app with a file-system reference in the Launch Services database.

Deprecated

### Deprecated Result Codes

var kLSNotInitializedErr: OSStatus

Not currently used.

var kLSUnknownTypeErr: OSStatus

Not currently used.

var kLSDataTooOldErr: OSStatus

Not currently used.

var kLSNotRegisteredErr: OSStatus

Not currently used.

var kLSAppDoesNotClaimTypeErr: OSStatus

Not currently used.

var kLSAppDoesNotSupportSchemeWarning: OSStatus

Not currently used.

var kLSNoRegistrationInfoErr: OSStatus

Not currently used.

var kLSNoClassicEnvironmentErr: OSStatus

Not currently used.

