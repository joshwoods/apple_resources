

- ColorSync
-  ColorSyncIterateInstalledProfiles(\_:\_:\_:\_:) 

Function

# ColorSyncIterateInstalledProfiles(\_:\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 13.0+macOS 10.13+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func ColorSyncIterateInstalledProfiles(
    _ callBack: ColorSyncProfileIterateCallback?,
    _ seed: UnsafeMutablePointer?,
    _ userInfo: UnsafeMutableRawPointer?,
    _ error: UnsafeMutablePointer?>?
)
```

## See Also

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

func ColorSyncProfileContainsTag(ColorSyncProfile!, CFString!) -> Bool

func ColorSyncProfileCopyData(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFData>!

func ColorSyncProfileCopyDescriptionString(ColorSyncProfile!) -> Unmanaged&lt;CFString>?

func ColorSyncProfileCopyHeader(ColorSyncProfile!) -> Unmanaged&lt;CFData>!

