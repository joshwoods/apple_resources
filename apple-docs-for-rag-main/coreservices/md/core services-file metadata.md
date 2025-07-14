

- Core Services
-  File Metadata 

API Collection

# File Metadata

Search for files based on data that is part of the file or file system.

## Topics

### Opaque Types

MDSchema

MDItem

### Structures

struct MDExporterInterfaceStruct

struct MDImporterBundleWrapperURLInterfaceStruct

struct MDImporterInterfaceStruct

struct MDImporterURLInterfaceStruct

struct MDLabelDomain

struct MDQuerySortOptionFlags

### Classes

class MDLabel

### Data Types

MDQuery

### Constants

let kMDItemApplicationCategories: CFString!

let kMDItemCameraOwner: CFString!

let kMDItemContentTypeTree: CFString!

let kMDItemDateAdded: CFString!

let kMDItemDownloadedDate: CFString!

let kMDItemEditors: CFString!

let kMDItemExecutableArchitectures: CFString!

let kMDItemExecutablePlatform: CFString!

let kMDItemFocalLength35mm: CFString!

let kMDItemGPSAreaInformation: CFString!

let kMDItemGPSDOP: CFString!

let kMDItemGPSDateStamp: CFString!

let kMDItemGPSDestBearing: CFString!

let kMDItemGPSDestDistance: CFString!

let kMDItemGPSDestLatitude: CFString!

let kMDItemGPSDestLongitude: CFString!

let kMDItemGPSDifferental: CFString!

let kMDItemGPSMapDatum: CFString!

let kMDItemGPSMeasureMode: CFString!

let kMDItemGPSProcessingMethod: CFString!

let kMDItemGPSStatus: CFString!

let kMDItemHTMLContent: CFString!

let kMDItemIsApplicationManaged: CFString!

let kMDItemIsLikelyJunk: CFString!

let kMDItemLensModel: CFString!

let kMDLabelAddedNotification: CFString!

var kMDLabelBundleURL: Unmanaged&lt;CFString>!

let kMDLabelChangedNotification: CFString!

var kMDLabelContentChangeDate: Unmanaged&lt;CFString>!

var kMDLabelDisplayName: Unmanaged&lt;CFString>!

var kMDLabelIconData: Unmanaged&lt;CFString>!

var kMDLabelIconUUID: Unmanaged&lt;CFString>!

var kMDLabelIsMutuallyExclusiveSetMember: Unmanaged&lt;CFString>!

var kMDLabelKind: Unmanaged&lt;CFString>!

var kMDLabelKindIsMutuallyExclusiveSetKey: Unmanaged&lt;CFString>!

var kMDLabelKindVisibilityKey: Unmanaged&lt;CFString>!

var kMDLabelLocalDomain: MDLabelDomain

let kMDLabelRemovedNotification: CFString!

var kMDLabelSetsFinderColor: Unmanaged&lt;CFString>!

var kMDLabelUUID: Unmanaged&lt;CFString>!

var kMDLabelUserDomain: MDLabelDomain

var kMDLabelVisibility: Unmanaged&lt;CFString>!

var kMDPrivateVisibility: Unmanaged&lt;CFString>!

var kMDPublicVisibility: Unmanaged&lt;CFString>!

var kMDQueryAllowFSTranslation: MDQueryOptionFlags

var kMDQueryReverseSortOrderFlag: MDQuerySortOptionFlags

var kMDQuerySynchronous: MDQueryOptionFlags

Specifies that a query should block during the initial gather phase. The query’s run loop will run in the default mode. If this option is not specified the query function returns immediately after starting the query asynchronously.

var kMDQueryWantsUpdates: MDQueryOptionFlags

## See Also

### Related Documentation

File Metadata Search Programming Guide

