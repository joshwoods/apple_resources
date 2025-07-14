

- ColorSync
-  ColorSync Functions 

API Collection

# ColorSync Functions

## Topics

### Functions

func ColorSyncAPIVersion() -> UInt32

func ColorSyncCreateCodeFragment(CFArray!, CFDictionary!) -> Unmanaged&lt;CFTypeRef>!

func ColorSyncIterateInstalledProfilesWithOptions(ColorSyncProfileIterateCallback?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?, CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

func ColorSyncProfileIsHLGBased(ColorSyncProfile!) -> Bool

func ColorSyncProfileIsMatrixBased(ColorSyncProfile!) -> Bool

func ColorSyncProfileIsPQBased(ColorSyncProfile!) -> Bool

func ColorSyncProfileIsWideGamut(ColorSyncProfile!) -> Bool

func ColorSyncTransformGetProfileSequence(ColorSyncTransform!) -> Unmanaged&lt;CFArray>?

### Additional functions

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

## See Also

### Reference

ColorSync Constants

