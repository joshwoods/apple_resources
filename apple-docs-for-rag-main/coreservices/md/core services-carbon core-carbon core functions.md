

- Core Services
- Carbon Core
-  Carbon Core Functions 

API Collection

# Carbon Core Functions

## Topics

### Functions

func AcquireIconRef(IconRef!) -> OSErrDeprecated

func CompositeIconRef(IconRef!, IconRef!, UnsafeMutablePointer&lt;IconRef?>!) -> OSErrDeprecated

func CreateCompDescriptor(DescType, UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a comparison descriptor that specifies how to compare one or more Apple event objects with either another Apple event object or a descriptor.

func CreateLogicalDescriptor(UnsafeMutablePointer&lt;AEDescList>!, DescType, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a logical descriptor that specifies a logical operator and one or more logical terms for the Apple Event Manager to evaluate.

func CreateObjSpecifier(DescType, UnsafeMutablePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Assembles an object specifier that identifies one or more Apple event objects, from other descriptors.

func CreateOffsetDescriptor(Int, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates an offset descriptor that specifies the position of an element in relation to the beginning or end of its container.

func CreateRangeDescriptor(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, Bool, UnsafeMutablePointer&lt;AEDesc>!) -> OSErr

Creates a range descriptor that specifies a series of consecutive elements in the same container.

func DCSCopyTextDefinition(DCSDictionary?, CFString, CFRange) -> Unmanaged&lt;CFString>?

Returns the definition associated with the provided text range.

func DCSGetTermRangeInString(DCSDictionary?, CFString, CFIndex) -> CFRange

Determines the range of the longest word or phrase with respect to an offset.

func DisposeAECoerceDescUPP(AECoerceDescUPP!)

Disposes of a universal procedure pointer to a function that coerces data stored in a descriptor.

func DisposeAECoercePtrUPP(AECoercePtrUPP!)

Disposes of a universal procedure pointer to a function that coerces data stored in a buffer.

func DisposeAEDisposeExternalUPP(AEDisposeExternalUPP!)

Disposes of a universal procedure pointer to a function that disposes of data supplied to the `AECreateDescFromExternalPtr` function.

func DisposeAEEventHandlerUPP(AEEventHandlerUPP!)

Disposes of a universal procedure pointer to an event handler function.

func DisposeIndexToUCStringUPP(IndexToUCStringUPP!)

func DisposeOSLAccessorUPP(OSLAccessorUPP!)

Disposes of a universal procedure pointer to an object accessor function.

func DisposeOSLAdjustMarksUPP(OSLAdjustMarksUPP!)

Disposes of a universal procedure pointer to an object callback adjust marks function.

func DisposeOSLCompareUPP(OSLCompareUPP!)

Disposes of a universal procedure pointer to an object callback comparison function.

func DisposeOSLCountUPP(OSLCountUPP!)

Disposes of a universal procedure pointer to an object callback count function.

func DisposeOSLDisposeTokenUPP(OSLDisposeTokenUPP!)

Disposes of a universal procedure pointer to an object callback dispose token function.

func DisposeOSLGetErrDescUPP(OSLGetErrDescUPP!)

Disposes of a universal procedure pointer to an object callback get error descriptor function.

func DisposeOSLGetMarkTokenUPP(OSLGetMarkTokenUPP!)

Disposes of a universal procedure pointer to an object callback get mark function.

func DisposeOSLMarkUPP(OSLMarkUPP!)

Disposes of a universal procedure pointer to an object callback mark function.

func GetCustomIconsEnabled(Int16, UnsafeMutablePointer&lt;DarwinBoolean>!) -> OSErrDeprecated

func GetIconRef(Int16, OSType, OSType, UnsafeMutablePointer&lt;IconRef?>!) -> OSErrDeprecated

func GetIconRefFromFileInfo(UnsafePointer&lt;FSRef>!, Int, UnsafePointer&lt;UniChar>!, FSCatalogInfoBitmap, UnsafePointer&lt;FSCatalogInfo>!, IconServicesUsageFlags, UnsafeMutablePointer&lt;IconRef?>!, UnsafeMutablePointer&lt;Int16>!) -> OSStatusDeprecated

func GetIconRefFromFolder(Int16, Int32, Int32, Int8, Int8, UnsafeMutablePointer&lt;IconRef?>!) -> OSErrDeprecated

func GetIconRefFromIconFamilyPtr(UnsafePointer&lt;IconFamilyResource>!, Size, UnsafeMutablePointer&lt;IconRef?>!) -> OSStatusDeprecated

func GetIconRefFromTypeInfo(OSType, OSType, CFString!, CFString!, IconServicesUsageFlags, UnsafeMutablePointer&lt;IconRef?>!) -> OSErrDeprecated

func GetIconRefOwners(IconRef!, UnsafeMutablePointer&lt;UInt16>!) -> OSErrDeprecated

func InvokeAECoerceDescUPP(UnsafePointer&lt;AEDesc>!, DescType, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!, AECoerceDescUPP!) -> OSErr

Calls a universal procedure pointer to a function that coerces data stored in a descriptor.

func InvokeAECoercePtrUPP(DescType, UnsafeRawPointer!, Size, DescType, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!, AECoercePtrUPP!) -> OSErr

Calls a universal procedure pointer to a function that coerces data stored in a buffer.

func InvokeAEDisposeExternalUPP(UnsafeRawPointer!, Size, SRefCon!, AEDisposeExternalUPP!)

Calls a dispose external universal procedure pointer.

func InvokeAEEventHandlerUPP(UnsafePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!, SRefCon!, AEEventHandlerUPP!) -> OSErr

Calls an event handler universal procedure pointer.

func InvokeIndexToUCStringUPP(UInt32, UnsafeMutableRawPointer!, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!, UnsafeMutablePointer&lt;UCTypeSelectOptions>!, IndexToUCStringUPP!) -> Bool

func InvokeOSLAccessorUPP(DescType, UnsafePointer&lt;AEDesc>!, DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, SRefCon!, OSLAccessorUPP!) -> OSErr

Calls an object accessor universal procedure pointer.

func InvokeOSLAdjustMarksUPP(Int, Int, UnsafePointer&lt;AEDesc>!, OSLAdjustMarksUPP!) -> OSErr

Calls an object callback adjust marks universal procedure pointer.

func InvokeOSLCompareUPP(DescType, UnsafePointer&lt;AEDesc>!, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;DarwinBoolean>!, OSLCompareUPP!) -> OSErr

Calls an object callback comparison universal procedure pointer.

func InvokeOSLCountUPP(DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;Int>!, OSLCountUPP!) -> OSErr

Calls an object callback count universal procedure pointer.

func InvokeOSLDisposeTokenUPP(UnsafeMutablePointer&lt;AEDesc>!, OSLDisposeTokenUPP!) -> OSErr

Calls an object callback dispose token universal procedure pointer.

func InvokeOSLGetErrDescUPP(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AEDesc>?>!, OSLGetErrDescUPP!) -> OSErr

Calls an object callback get error descriptor universal procedure pointer.

func InvokeOSLGetMarkTokenUPP(UnsafePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, OSLGetMarkTokenUPP!) -> OSErr

Calls an object callback get mark universal procedure pointer.

func InvokeOSLMarkUPP(UnsafePointer&lt;AEDesc>!, UnsafePointer&lt;AEDesc>!, Int, OSLMarkUPP!) -> OSErr

Calls an object callback mark universal procedure pointer.

func IsDataAvailableInIconRef(OSType, IconRef!) -> BoolDeprecated

func IsIconRefComposite(IconRef!, UnsafeMutablePointer&lt;IconRef?>!, UnsafeMutablePointer&lt;IconRef?>!) -> OSErrDeprecated

func IsValidIconRef(IconRef!) -> BoolDeprecated

func LSSetItemAttribute(UnsafePointer&lt;FSRef>!, LSRolesMask, CFString!, CFTypeRef!) -> OSStatusDeprecated

func LSSharedFileListAddObserver(LSSharedFileList?, CFRunLoop, CFString, LSSharedFileListChangedProcPtr, UnsafeMutableRawPointer?)Deprecated

func LSSharedFileListCopyProperty(LSSharedFileList, CFString) -> Unmanaged&lt;CFTypeRef>?Deprecated

func LSSharedFileListCopySnapshot(LSSharedFileList, UnsafeMutablePointer&lt;UInt32>?) -> Unmanaged&lt;CFArray>?Deprecated

func LSSharedFileListCreate(CFAllocator?, CFString, CFTypeRef?) -> Unmanaged&lt;LSSharedFileList>?Deprecated

func LSSharedFileListGetSeedValue(LSSharedFileList) -> UInt32Deprecated

func LSSharedFileListGetTypeID() -> CFTypeIDDeprecated

func LSSharedFileListInsertItemFSRef(LSSharedFileList, LSSharedFileListItem, CFString?, IconRef?, UnsafePointer&lt;FSRef>, CFDictionary?, CFArray?) -> LSSharedFileListItem?Deprecated

func LSSharedFileListInsertItemURL(LSSharedFileList, LSSharedFileListItem, CFString?, IconRef?, CFURL, CFDictionary?, CFArray?) -> LSSharedFileListItem?Deprecated

func LSSharedFileListItemCopyDisplayName(LSSharedFileListItem) -> Unmanaged&lt;CFString>Deprecated

func LSSharedFileListItemCopyIconRef(LSSharedFileListItem) -> IconRefDeprecated

func LSSharedFileListItemCopyProperty(LSSharedFileListItem, CFString) -> Unmanaged&lt;CFTypeRef>?Deprecated

func LSSharedFileListItemCopyResolvedURL(LSSharedFileListItem, LSSharedFileListResolutionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?Deprecated

func LSSharedFileListItemGetID(LSSharedFileListItem) -> UInt32Deprecated

func LSSharedFileListItemGetTypeID() -> CFTypeIDDeprecated

func LSSharedFileListItemMove(LSSharedFileList, LSSharedFileListItem, LSSharedFileListItem) -> OSStatusDeprecated

func LSSharedFileListItemRemove(LSSharedFileList, LSSharedFileListItem) -> OSStatusDeprecated

func LSSharedFileListItemResolve(LSSharedFileListItem, LSSharedFileListResolutionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>?, UnsafeMutablePointer&lt;FSRef>?) -> OSStatusDeprecated

func LSSharedFileListItemSetProperty(LSSharedFileListItem, CFString, CFTypeRef) -> OSStatusDeprecated

func LSSharedFileListRemoveAllItems(LSSharedFileList) -> OSStatusDeprecated

func LSSharedFileListRemoveObserver(LSSharedFileList, CFRunLoop, CFString, LSSharedFileListChangedProcPtr, UnsafeMutableRawPointer?)Deprecated

func LSSharedFileListSetAuthorization(LSSharedFileList, AuthorizationRef) -> OSStatusDeprecated

func LSSharedFileListSetProperty(LSSharedFileList, CFString, CFTypeRef?) -> OSStatusDeprecated

func MDCopyLabelKinds() -> CFArray!

func MDCopyLabelWithUUID(CFUUID!) -> MDLabel!

func MDCopyLabelsMatchingExpression(CFString!) -> CFArray!

func MDCopyLabelsWithKind(CFString!) -> CFArray!

func MDItemCopyLabels(MDItem!) -> CFArray!

func MDItemRemoveLabel(MDItem!, MDLabel!) -> Bool

func MDItemSetLabel(MDItem!, MDLabel!) -> Bool

func MDItemsCopyAttributes(CFArray!, CFArray!) -> CFArray!

func MDItemsCreateWithURLs(CFAllocator!, CFArray!) -> CFArray!

func MDLabelCopyAttribute(MDLabel!, CFString!) -> CFTypeRef!

func MDLabelCopyAttributeName(MDLabel!) -> CFString!

func MDLabelCreate(CFAllocator!, CFString!, CFString!, MDLabelDomain) -> MDLabel!

func MDLabelDelete(MDLabel!) -> Bool

func MDLabelGetTypeID() -> CFTypeID

func MDLabelSetAttributes(MDLabel!, CFDictionary!) -> Bool

func MDQueryCreateForItems(CFAllocator!, CFString!, CFArray!, CFArray!, CFArray!) -> MDQuery!

func MDQueryGetSortOptionFlagsForAttribute(MDQuery!, CFString!) -> UInt32

func MDQuerySetSortOptionFlagsForAttribute(MDQuery!, CFString!, UInt32) -> Bool

func MDQuerySetSortOrder(MDQuery!, CFArray!) -> Bool

func NewAECoerceDescUPP(AECoerceDescProcPtr!) -> AECoerceDescUPP!

Creates a new universal procedure pointer to a function that coerces data stored in a descriptor.

func NewAECoercePtrUPP(AECoercePtrProcPtr!) -> AECoercePtrUPP!

Creates a new universal procedure pointer to a function that coerces data stored in a buffer.

func NewAEDisposeExternalUPP(AEDisposeExternalProcPtr!) -> AEDisposeExternalUPP!

Creates a new universal procedure pointer to a function that disposes of data stored in a buffer.

func NewAEEventHandlerUPP(AEEventHandlerProcPtr!) -> AEEventHandlerUPP!

Creates a new universal procedure pointer to an event handler function.

func NewIndexToUCStringUPP(IndexToUCStringProcPtr!) -> IndexToUCStringUPP!

func NewOSLAccessorUPP(OSLAccessorProcPtr!) -> OSLAccessorUPP!

Creates a new universal procedure pointer to an object accessor function.

func NewOSLAdjustMarksUPP(OSLAdjustMarksProcPtr!) -> OSLAdjustMarksUPP!

Creates a new universal procedure pointer to an object callback adjust marks function.

func NewOSLCompareUPP(OSLCompareProcPtr!) -> OSLCompareUPP!

Creates a new universal procedure pointer to an object callback comparison function.

func NewOSLCountUPP(OSLCountProcPtr!) -> OSLCountUPP!

Creates a new universal procedure pointer to an object callback count function.

func NewOSLDisposeTokenUPP(OSLDisposeTokenProcPtr!) -> OSLDisposeTokenUPP!

Creates a new universal procedure pointer to an object callback dispose token function.

func NewOSLGetErrDescUPP(OSLGetErrDescProcPtr!) -> OSLGetErrDescUPP!

Creates a new universal procedure pointer to an object callback get error descriptor function.

func NewOSLGetMarkTokenUPP(OSLGetMarkTokenProcPtr!) -> OSLGetMarkTokenUPP!

Creates a new universal procedure pointer to an object callback get mark function.

func NewOSLMarkUPP(OSLMarkProcPtr!) -> OSLMarkUPP!

Creates a new universal procedure pointer to an object callback mark function.

func OverrideIconRef(IconRef!, IconRef!) -> OSErrDeprecated

func ReadIconFromFSRef(UnsafePointer&lt;FSRef>!, UnsafeMutablePointer&lt;IconFamilyHandle?>!) -> OSStatusDeprecated

func RegisterIconRefFromFSRef(OSType, OSType, UnsafePointer&lt;FSRef>!, UnsafeMutablePointer&lt;IconRef?>!) -> OSStatusDeprecated

func RegisterIconRefFromIconFamily(OSType, OSType, IconFamilyHandle!, UnsafeMutablePointer&lt;IconRef?>!) -> OSErrDeprecated

func ReleaseIconRef(IconRef!) -> OSErrDeprecated

func RemoveIconRefOverride(IconRef!) -> OSErrDeprecated

func SetCustomIconsEnabled(Int16, Bool) -> OSErrDeprecated

func UCTypeSelectAddKeyToSelector(UCTypeSelectRef!, CFString!, Double, UnsafeMutablePointer&lt;DarwinBoolean>!) -> OSStatus

func UCTypeSelectCompare(UCTypeSelectRef!, CFString!, UnsafeMutablePointer&lt;UCTypeSelectCompareResult>!) -> OSStatus

func UCTypeSelectCreateSelector(LocaleRef!, LocaleOperationVariant, UCCollateOptions, UnsafeMutablePointer&lt;UCTypeSelectRef?>!) -> OSStatus

func UCTypeSelectFindItem(UCTypeSelectRef!, UInt32, UnsafeMutableRawPointer!, UnsafeMutableRawPointer!, IndexToUCStringUPP!, UnsafeMutablePointer&lt;UInt32>!) -> OSStatus

func UCTypeSelectFlushSelectorData(UCTypeSelectRef!) -> OSStatus

func UCTypeSelectReleaseSelector(UnsafeMutablePointer&lt;UCTypeSelectRef?>!) -> OSStatus

func UCTypeSelectWalkList(UCTypeSelectRef!, CFString!, UCTSWalkDirection, UInt32, UnsafeMutableRawPointer!, UnsafeMutableRawPointer!, IndexToUCStringUPP!, UnsafeMutablePointer&lt;UInt32>!) -> OSStatus

func UCTypeSelectWouldResetBuffer(UCTypeSelectRef!, CFString!, Double) -> Bool

func UTCreateStringForOSType(OSType) -> Unmanaged&lt;CFString>

Encodes an `OSType` into a string suitable for use as a tag argument.

Deprecated

func UTGetOSTypeFromString(CFString) -> OSType

Decodes a tag string into an OSType.

Deprecated

func UTTypeConformsTo(CFString, CFString) -> Bool

Returns whether a uniform type identifier conforms to another uniform type identifier.

Deprecated

func UTTypeCopyAllTagsWithClass(CFString, CFString) -> Unmanaged&lt;CFArray>?Deprecated

func UTTypeCopyDeclaration(CFString) -> Unmanaged&lt;CFDictionary>?

Returns a uniform type’s declaration.

Deprecated

func UTTypeCopyDeclaringBundleURL(CFString) -> Unmanaged&lt;CFURL>?

Returns the location of a bundle containing the declaration for a type.

Deprecated

func UTTypeCopyDescription(CFString) -> Unmanaged&lt;CFString>?

Returns the localized, user-readable type description string associated with a uniform type identifier.

Deprecated

func UTTypeCopyPreferredTagWithClass(CFString, CFString) -> Unmanaged&lt;CFString>?

Translates a uniform type identifier to a list of tags in a different type classification method.

Deprecated

func UTTypeCreateAllIdentifiersForTag(CFString, CFString, CFString?) -> Unmanaged&lt;CFArray>?

Creates an array of all uniform type identifiers for the type indicated by the specified tag.

Deprecated

func UTTypeCreatePreferredIdentifierForTag(CFString, CFString, CFString?) -> Unmanaged&lt;CFString>?

Creates a uniform type identifier for the type indicated by the specified tag.

Deprecated

func UTTypeEqual(CFString, CFString) -> Bool

Returns whether two uniform type identifiers are equal.

Deprecated

func UTTypeIsDeclared(CFString) -> BoolDeprecated

func UTTypeIsDynamic(CFString) -> BoolDeprecated

func UnregisterIconRef(OSType, OSType) -> OSErrDeprecated

func UpdateIconRef(IconRef!) -> OSErrDeprecated

func vAEBuildAppleEvent(AEEventClass, AEEventID, DescType, UnsafeRawPointer!, Size, Int16, Int32, UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildAppleEvent` in a wrapper routine.

func vAEBuildDesc(UnsafeMutablePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildDesc` in your own wrapper routines.

func vAEBuildParameters(UnsafeMutablePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AEBuildError>!, UnsafePointer&lt;CChar>!, CVaListPointer) -> OSStatus

Allows you to encapsulate calls to `AEBuildParameters` in your own `stdarg`-style wrapper routines, using techniques similar to those allowed by vsprintf.

func AEDeterminePermissionToAutomateTarget(UnsafePointer&lt;AEAddressDesc>!, AEEventClass, AEEventID, Bool) -> OSStatus

func AEUnflattenDescFromBytes(UnsafeRawPointer!, Int, UnsafeMutablePointer&lt;AEDesc>!) -> OSStatus

func MDItemGetCacheFileDescriptors(CFArray!, ((CFArray?) -> Void)!)

## See Also

### Other Reference

Carbon Core Structures

Carbon Core Enumerations

Carbon Core Data Types

