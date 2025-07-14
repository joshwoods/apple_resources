

- Application Services
-  ApplicationServices Functions 

API Collection

# ApplicationServices Functions

## Topics

### Functions

func CGDisplayCreateUUIDFromDisplayID(UInt32) -> Unmanaged&lt;CFUUID>!

func CGDisplayGetDisplayIDFromUUID(CFUUID!) -> UInt32

func ColorSyncCMMCopyCMMIdentifier(ColorSyncCMM!) -> Unmanaged&lt;CFString>?

func ColorSyncCMMCopyLocalizedName(ColorSyncCMM!) -> Unmanaged&lt;CFString>?

func ColorSyncCMMCreate(CFBundle!) -> Unmanaged&lt;ColorSyncCMM>?

func ColorSyncCMMGetBundle(ColorSyncCMM!) -> Unmanaged&lt;CFBundle>?

func ColorSyncCMMGetTypeID() -> CFTypeID

func ColorSyncDeviceCopyDeviceInfo(CFString!, CFUUID!) -> Unmanaged&lt;CFDictionary>?

func ColorSyncDeviceSetCustomProfiles(CFString!, CFUUID!, CFDictionary!) -> Bool

func ColorSyncIterateDeviceProfiles(ColorSyncDeviceProfileIterateCallback!, UnsafeMutableRawPointer?)

func ColorSyncIterateInstalledCMMs(ColorSyncCMMIterateCallback!, UnsafeMutableRawPointer?)

func ColorSyncIterateInstalledProfiles(ColorSyncProfileIterateCallback?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

func ColorSyncProfileContainsTag(ColorSyncProfile!, CFString!) -> Bool

func ColorSyncProfileCopyData(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFData>!

func ColorSyncProfileCopyDescriptionString(ColorSyncProfile!) -> Unmanaged&lt;CFString>?

func ColorSyncProfileCopyHeader(ColorSyncProfile!) -> Unmanaged&lt;CFData>!

func ColorSyncProfileCopyTag(ColorSyncProfile!, CFString!) -> Unmanaged&lt;CFData>?

func ColorSyncProfileCopyTagSignatures(ColorSyncProfile!) -> Unmanaged&lt;CFArray>?

func ColorSyncProfileCreate(CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;ColorSyncProfile>?

func ColorSyncProfileCreateDeviceProfile(CFString!, CFUUID!, CFTypeRef!) -> Unmanaged&lt;ColorSyncProfile>?

func ColorSyncProfileCreateDisplayTransferTablesFromVCGT(ColorSyncProfile!, UnsafeMutablePointer&lt;Int>!) -> Unmanaged&lt;CFData>?

func ColorSyncProfileCreateLink(CFArray!, CFDictionary?) -> Unmanaged&lt;ColorSyncProfile>?

func ColorSyncProfileCreateMutable() -> Unmanaged&lt;ColorSyncMutableProfile>?

func ColorSyncProfileCreateMutableCopy(ColorSyncProfile!) -> Unmanaged&lt;ColorSyncMutableProfile>?

func ColorSyncProfileCreateWithDisplayID(UInt32) -> Unmanaged&lt;ColorSyncProfile>?

func ColorSyncProfileCreateWithName(CFString!) -> Unmanaged&lt;ColorSyncProfile>?

func ColorSyncProfileCreateWithURL(CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;ColorSyncProfile>?

func ColorSyncProfileEstimateGamma(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Float

func ColorSyncProfileEstimateGammaWithDisplayID(Int32, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Float

func ColorSyncProfileGetDisplayTransferFormulaFromVCGT(ColorSyncProfile!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!, UnsafeMutablePointer&lt;Float>!) -> Bool

func ColorSyncProfileGetMD5(ColorSyncProfile!) -> ColorSyncMD5

func ColorSyncProfileGetTypeID() -> CFTypeID

func ColorSyncProfileGetURL(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>!

func ColorSyncProfileInstall(ColorSyncProfile!, CFString!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

func ColorSyncProfileRemoveTag(ColorSyncMutableProfile!, CFString!)

func ColorSyncProfileSetHeader(ColorSyncMutableProfile!, CFData!)

func ColorSyncProfileSetTag(ColorSyncMutableProfile!, CFString!, CFData!)

func ColorSyncProfileUninstall(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

func ColorSyncProfileVerify(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

func ColorSyncRegisterDevice(CFString!, CFUUID!, CFDictionary!) -> Bool

func ColorSyncTransformConvert(ColorSyncTransform!, Int, Int, UnsafeMutableRawPointer!, ColorSyncDataDepth, ColorSyncDataLayout, Int, UnsafeRawPointer!, ColorSyncDataDepth, ColorSyncDataLayout, Int, CFDictionary?) -> Bool

func ColorSyncTransformCopyProperty(ColorSyncTransform!, CFTypeRef!, CFDictionary?) -> Unmanaged&lt;CFTypeRef>?

func ColorSyncTransformCreate(CFArray?, CFDictionary?) -> Unmanaged&lt;ColorSyncTransform>?

func ColorSyncTransformGetTypeID() -> CFTypeID

func ColorSyncTransformSetProperty(ColorSyncTransform!, CFTypeRef!, CFTypeRef?)

func ColorSyncUnregisterDevice(CFString!, CFUUID!) -> Bool

func DisposeIconActionUPP(IconActionUPP!)

func DisposeIconGetterUPP(IconGetterUPP!)

func GetIconFamilyData(IconFamilyHandle!, OSType, Handle!) -> OSErr

func GetIconRefVariant(IconRef!, OSType, UnsafeMutablePointer&lt;IconTransformType>!) -> IconRef!

func HIShapeContainsPoint(HIShape!, UnsafePointer&lt;CGPoint>!) -> Bool

func HIShapeCreateCopy(HIShape!) -> Unmanaged&lt;HIShape>!

func HIShapeCreateDifference(HIShape!, HIShape!) -> Unmanaged&lt;HIShape>!

func HIShapeCreateEmpty() -> Unmanaged&lt;HIShape>!

func HIShapeCreateIntersection(HIShape!, HIShape!) -> Unmanaged&lt;HIShape>!

func HIShapeCreateMutable() -> Unmanaged&lt;HIMutableShape>!

func HIShapeCreateMutableCopy(HIShape!) -> Unmanaged&lt;HIMutableShape>!

func HIShapeCreateMutableWithRect(UnsafePointer&lt;CGRect>!) -> Unmanaged&lt;HIMutableShape>!

func HIShapeCreateUnion(HIShape!, HIShape!) -> Unmanaged&lt;HIShape>!

func HIShapeCreateWithQDRgn(RgnHandle!) -> Unmanaged&lt;HIShape>!

func HIShapeCreateWithRect(UnsafePointer&lt;CGRect>!) -> Unmanaged&lt;HIShape>!

func HIShapeCreateXor(HIShape!, HIShape!) -> Unmanaged&lt;HIShape>!

func HIShapeDifference(HIShape!, HIShape!, HIMutableShape!) -> OSStatus

func HIShapeEnumerate(HIShape!, OptionBits, HIShapeEnumerateProcPtr!, UnsafeMutableRawPointer!) -> OSStatus

func HIShapeGetAsQDRgn(HIShape!, RgnHandle!) -> OSStatus

func HIShapeGetBounds(HIShape!, UnsafeMutablePointer&lt;CGRect>!) -> UnsafeMutablePointer&lt;CGRect>!

func HIShapeGetTypeID() -> CFTypeID

func HIShapeInset(HIMutableShape!, CGFloat, CGFloat) -> OSStatus

func HIShapeIntersect(HIShape!, HIShape!, HIMutableShape!) -> OSStatus

func HIShapeIntersectsRect(HIShape!, UnsafePointer&lt;CGRect>!) -> Bool

func HIShapeIsEmpty(HIShape!) -> Bool

func HIShapeIsRectangular(HIShape!) -> Bool

func HIShapeOffset(HIMutableShape!, CGFloat, CGFloat) -> OSStatus

func HIShapeReplacePathInCGContext(HIShape!, CGContext!) -> OSStatus

func HIShapeSetEmpty(HIMutableShape!) -> OSStatus

func HIShapeSetWithShape(HIMutableShape!, HIShape!) -> OSStatus

func HIShapeUnion(HIShape!, HIShape!, HIMutableShape!) -> OSStatus

func HIShapeUnionWithRect(HIMutableShape!, UnsafePointer&lt;CGRect>!) -> OSStatus

func HIShapeXor(HIShape!, HIShape!, HIMutableShape!) -> OSStatus

func IconRefContainsCGPoint(UnsafePointer&lt;CGPoint>!, UnsafePointer&lt;CGRect>!, IconAlignmentType, IconServicesUsageFlags, IconRef!) -> Bool

func IconRefIntersectsCGRect(UnsafePointer&lt;CGRect>!, UnsafePointer&lt;CGRect>!, IconAlignmentType, IconServicesUsageFlags, IconRef!) -> Bool

func IconRefToHIShape(UnsafePointer&lt;CGRect>!, IconAlignmentType, IconServicesUsageFlags, IconRef!) -> Unmanaged&lt;HIShape>!

func IconRefToIconFamily(IconRef!, IconSelectorValue, UnsafeMutablePointer&lt;IconFamilyHandle?>!) -> OSErr

func InvokeIconActionUPP(ResType, UnsafeMutablePointer&lt;Handle?>!, UnsafeMutableRawPointer!, IconActionUPP!) -> OSErr

func InvokeIconGetterUPP(ResType, UnsafeMutableRawPointer!, IconGetterUPP!) -> Handle!

func IsIconRefMaskEmpty(IconRef!) -> Bool

func NewIconActionUPP(IconActionProcPtr!) -> IconActionUPP!

func NewIconGetterUPP(IconGetterProcPtr!) -> IconGetterUPP!

func PMPrinterCopyState(PMPrinter, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

func PMPrinterSendCommand(PMPrinter, CFString, CFString?, CFDictionary?) -> OSStatus

func PasteboardClear(Pasteboard) -> OSStatus

func PasteboardCopyItemFlavorData(Pasteboard, PasteboardItemID, CFString, UnsafeMutablePointer&lt;CFData?>) -> OSStatus

func PasteboardCopyItemFlavors(Pasteboard, PasteboardItemID, UnsafeMutablePointer&lt;CFArray?>) -> OSStatus

func PasteboardCopyName(Pasteboard, UnsafeMutablePointer&lt;CFString?>) -> OSStatus

func PasteboardCopyPasteLocation(Pasteboard, UnsafeMutablePointer&lt;CFURL?>) -> OSStatus

func PasteboardCreate(CFString?, UnsafeMutablePointer&lt;Pasteboard?>) -> OSStatus

func PasteboardGetItemCount(Pasteboard, UnsafeMutablePointer&lt;Int>) -> OSStatus

func PasteboardGetItemFlavorFlags(Pasteboard, PasteboardItemID, CFString, UnsafeMutablePointer&lt;PasteboardFlavorFlags>) -> OSStatus

func PasteboardGetItemIdentifier(Pasteboard, CFIndex, UnsafeMutablePointer&lt;PasteboardItemID?>) -> OSStatus

func PasteboardGetTypeID() -> CFTypeID

func PasteboardPutItemFlavor(Pasteboard, PasteboardItemID, CFString, CFData?, PasteboardFlavorFlags) -> OSStatus

func PasteboardResolvePromises(Pasteboard) -> OSStatus

func PasteboardSetPasteLocation(Pasteboard, CFURL) -> OSStatus

func PasteboardSetPromiseKeeper(Pasteboard, PasteboardPromiseKeeperProcPtr, UnsafeMutableRawPointer?) -> OSStatus

func PasteboardSynchronize(Pasteboard) -> PasteboardSyncFlags

func PlotIconRefInContext(CGContext!, UnsafePointer&lt;CGRect>!, IconAlignmentType, IconTransformType, UnsafePointer&lt;RGBColor>!, PlotIconRefFlags, IconRef!) -> OSStatus

func SetIconFamilyData(IconFamilyHandle!, OSType, Handle!) -> OSErr

func TransformProcessType(UnsafePointer&lt;ProcessSerialNumber>!, ProcessApplicationTransformState) -> OSStatus

func TranslationCopyDestinationType(Translation!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

func TranslationCopySourceType(Translation!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatus

func TranslationCreate(CFString!, CFString!, TranslationFlags, UnsafeMutablePointer&lt;Unmanaged&lt;Translation>?>!) -> OSStatus

func TranslationCreateWithSourceArray(CFArray!, TranslationFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFArray>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!) -> OSStatus

func TranslationGetTranslationFlags(Translation!, UnsafeMutablePointer&lt;TranslationFlags>!) -> OSStatus

func TranslationGetTypeID() -> CFTypeID

func TranslationPerformForData(Translation!, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!) -> OSStatus

func TranslationPerformForFile(Translation!, UnsafePointer&lt;FSRef>!, UnsafePointer&lt;FSRef>!, CFString!, UnsafeMutablePointer&lt;FSRef>!) -> OSStatus

func TranslationPerformForURL(Translation!, CFURL!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>!) -> OSStatus

func ATSCreateFontQueryRunLoopSource(CFIndex, CFIndex, ATSFontQueryCallback!, UnsafePointer&lt;ATSFontQuerySourceContext>!) -> Unmanaged&lt;CFRunLoopSource>!Deprecated

func ATSFontActivateFromFileReference(UnsafePointer&lt;FSRef>!, ATSFontContext, ATSFontFormat, UnsafeMutableRawPointer!, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontContainerRef>!) -> OSStatusDeprecated

func ATSFontActivateFromMemory(LogicalAddress!, Int, ATSFontContext, ATSFontFormat, UnsafeMutableRawPointer!, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontContainerRef>!) -> OSStatusDeprecated

func ATSFontApplyFunction(ATSFontApplierFunction!, UnsafeMutableRawPointer!) -> OSStatusDeprecated

func ATSFontDeactivate(ATSFontContainerRef, UnsafeMutableRawPointer!, ATSOptionFlags) -> OSStatusDeprecated

func ATSFontFamilyApplyFunction(ATSFontFamilyApplierFunction!, UnsafeMutableRawPointer!) -> OSStatusDeprecated

func ATSFontFamilyFindFromName(CFString!, ATSOptionFlags) -> ATSFontFamilyRefDeprecated

func ATSFontFamilyFindFromQuickDrawName(ConstStr255Param!) -> ATSFontFamilyRefDeprecated

func ATSFontFamilyGetEncoding(ATSFontFamilyRef) -> TextEncodingDeprecated

func ATSFontFamilyGetGeneration(ATSFontFamilyRef) -> ATSGenerationDeprecated

func ATSFontFamilyGetName(ATSFontFamilyRef, ATSOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatusDeprecated

func ATSFontFamilyGetQuickDrawName(ATSFontFamilyRef, UnsafeMutablePointer&lt;UInt8>!) -> OSStatusDeprecated

func ATSFontFamilyIteratorCreate(ATSFontContext, UnsafePointer&lt;ATSFontFilter>!, UnsafeMutableRawPointer!, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontFamilyIterator?>!) -> OSStatusDeprecated

func ATSFontFamilyIteratorNext(ATSFontFamilyIterator!, UnsafeMutablePointer&lt;ATSFontFamilyRef>!) -> OSStatusDeprecated

func ATSFontFamilyIteratorRelease(UnsafeMutablePointer&lt;ATSFontFamilyIterator?>!) -> OSStatusDeprecated

func ATSFontFamilyIteratorReset(ATSFontContext, UnsafePointer&lt;ATSFontFilter>!, UnsafeMutableRawPointer!, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontFamilyIterator?>!) -> OSStatusDeprecated

func ATSFontFindFromContainer(ATSFontContainerRef, ATSOptionFlags, Int, UnsafeMutablePointer&lt;ATSFontRef>!, UnsafeMutablePointer&lt;Int>!) -> OSStatusDeprecated

func ATSFontFindFromName(CFString!, ATSOptionFlags) -> ATSFontRefDeprecated

func ATSFontFindFromPostScriptName(CFString!, ATSOptionFlags) -> ATSFontRefDeprecated

func ATSFontGetAutoActivationSettingForApplication(CFURL!) -> ATSFontAutoActivationSettingDeprecated

func ATSFontGetContainer(ATSFontRef, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontContainerRef>!) -> OSStatusDeprecated

func ATSFontGetContainerFromFileReference(UnsafePointer&lt;FSRef>!, ATSFontContext, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontContainerRef>!) -> OSStatusDeprecated

func ATSFontGetFileReference(ATSFontRef, UnsafeMutablePointer&lt;FSRef>!) -> OSStatusDeprecated

func ATSFontGetFontFamilyResource(ATSFontRef, Int, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> OSStatusDeprecated

func ATSFontGetGeneration(ATSFontRef) -> ATSGenerationDeprecated

func ATSFontGetGlobalAutoActivationSetting() -> ATSFontAutoActivationSettingDeprecated

func ATSFontGetHorizontalMetrics(ATSFontRef, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontMetrics>!) -> OSStatusDeprecated

func ATSFontGetName(ATSFontRef, ATSOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatusDeprecated

func ATSFontGetPostScriptName(ATSFontRef, ATSOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> OSStatusDeprecated

func ATSFontGetTable(ATSFontRef, FourCharCode, ByteOffset, Int, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> OSStatusDeprecated

func ATSFontGetTableDirectory(ATSFontRef, Int, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;Int>!) -> OSStatusDeprecated

func ATSFontGetVerticalMetrics(ATSFontRef, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontMetrics>!) -> OSStatusDeprecated

func ATSFontIsEnabled(ATSFontRef) -> BoolDeprecated

func ATSFontIteratorCreate(ATSFontContext, UnsafePointer&lt;ATSFontFilter>!, UnsafeMutableRawPointer!, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontIterator?>!) -> OSStatusDeprecated

func ATSFontIteratorNext(ATSFontIterator!, UnsafeMutablePointer&lt;ATSFontRef>!) -> OSStatusDeprecated

func ATSFontIteratorRelease(UnsafeMutablePointer&lt;ATSFontIterator?>!) -> OSStatusDeprecated

func ATSFontIteratorReset(ATSFontContext, UnsafePointer&lt;ATSFontFilter>!, UnsafeMutableRawPointer!, ATSOptionFlags, UnsafeMutablePointer&lt;ATSFontIterator?>!) -> OSStatusDeprecated

func ATSFontNotificationSubscribe(ATSNotificationCallback!, ATSFontNotifyOption, UnsafeMutableRawPointer!, UnsafeMutablePointer&lt;ATSFontNotificationRef?>!) -> OSStatusDeprecated

func ATSFontNotificationUnsubscribe(ATSFontNotificationRef!) -> OSStatusDeprecated

func ATSFontNotify(ATSFontNotifyAction, UnsafeMutableRawPointer!) -> OSStatusDeprecated

func ATSFontSetAutoActivationSettingForApplication(ATSFontAutoActivationSetting, CFURL!) -> OSStatusDeprecated

func ATSFontSetEnabled(ATSFontRef, ATSOptionFlags, Bool) -> OSStatusDeprecated

func ATSFontSetGlobalAutoActivationSetting(ATSFontAutoActivationSetting) -> OSStatusDeprecated

func ATSGetGeneration() -> ATSGenerationDeprecated

func AXTextMarkerCreate(CFAllocator?, UnsafePointer&lt;UInt8>, CFIndex) -> AXTextMarker

func AXTextMarkerGetBytePtr(AXTextMarker) -> UnsafePointer&lt;UInt8>

func AXTextMarkerGetLength(AXTextMarker) -> CFIndex

func AXTextMarkerGetTypeID() -> CFTypeID

func AXTextMarkerRangeCopyEndMarker(AXTextMarkerRange) -> AXTextMarker

func AXTextMarkerRangeCopyStartMarker(AXTextMarkerRange) -> AXTextMarker

func AXTextMarkerRangeCreate(CFAllocator?, AXTextMarker, AXTextMarker) -> AXTextMarkerRange

func AXTextMarkerRangeCreateWithBytes(CFAllocator?, UnsafePointer&lt;UInt8>, CFIndex, UnsafePointer&lt;UInt8>, CFIndex) -> AXTextMarkerRange

func AXTextMarkerRangeGetTypeID() -> CFTypeID

func DisposeSpeechDoneUPP(SpeechDoneUPP)Deprecated

func DisposeSpeechErrorUPP(SpeechErrorUPP)Deprecated

func DisposeSpeechPhonemeUPP(SpeechPhonemeUPP)Deprecated

func DisposeSpeechSyncUPP(SpeechSyncUPP)Deprecated

func DisposeSpeechTextDoneUPP(SpeechTextDoneUPP)Deprecated

func DisposeSpeechWordUPP(SpeechWordUPP)Deprecated

func GetSpeechInfo(SpeechChannel, OSType, UnsafeMutableRawPointer) -> OSErrDeprecated

func InvokeSpeechDoneUPP(SpeechChannel, SRefCon, SpeechDoneUPP)Deprecated

func InvokeSpeechErrorUPP(SpeechChannel, SRefCon, OSErr, Int, SpeechErrorUPP)Deprecated

func InvokeSpeechPhonemeUPP(SpeechChannel, SRefCon, Int16, SpeechPhonemeUPP)Deprecated

func InvokeSpeechSyncUPP(SpeechChannel, SRefCon, OSType, SpeechSyncUPP)Deprecated

func InvokeSpeechTextDoneUPP(SpeechChannel, SRefCon, UnsafeMutablePointer&lt;UnsafeRawPointer?>?, UnsafeMutablePointer&lt;UInt>, UnsafeMutablePointer&lt;Int32>, SpeechTextDoneUPP)Deprecated

func InvokeSpeechWordUPP(SpeechChannel, SRefCon, UInt, UInt16, SpeechWordUPP)Deprecated

func NewSpeechDoneUPP(SpeechDoneProcPtr) -> SpeechDoneUPPDeprecated

func NewSpeechErrorUPP(SpeechErrorProcPtr) -> SpeechErrorUPPDeprecated

func NewSpeechPhonemeUPP(SpeechPhonemeProcPtr) -> SpeechPhonemeUPPDeprecated

func NewSpeechSyncUPP(SpeechSyncProcPtr) -> SpeechSyncUPPDeprecated

func NewSpeechTextDoneUPP(SpeechTextDoneProcPtr) -> SpeechTextDoneUPPDeprecated

func NewSpeechWordUPP(SpeechWordProcPtr) -> SpeechWordUPPDeprecated

func SetSpeechInfo(SpeechChannel, OSType, UnsafeRawPointer?) -> OSErrDeprecated

func SpeakBuffer(SpeechChannel, UnsafeRawPointer, UInt, Int32) -> OSErrDeprecated

func SpeakString(ConstStr255Param) -> OSErrDeprecated

func SpeakText(SpeechChannel, UnsafeRawPointer, UInt) -> OSErrDeprecated

func TextToPhonemes(SpeechChannel, UnsafeRawPointer, UInt, Handle, UnsafeMutablePointer&lt;Int>) -> OSErrDeprecated

func UseDictionary(SpeechChannel, Handle) -> OSErrDeprecated

