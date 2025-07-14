

- ColorSync
-  ColorSyncRegisterDevice(\_:\_:\_:) 

Function

# ColorSyncRegisterDevice(\_:\_:\_:)

Mac Catalyst 13.0+macOS 10.13+

``` source
func ColorSyncRegisterDevice(
    _ deviceClass: CFString!,
    _ deviceID: CFUUID!,
    _ deviceInfo: CFDictionary!
) -> Bool
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

func ColorSyncIterateInstalledProfiles(ColorSyncProfileIterateCallback?, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?)

func ColorSyncProfileContainsTag(ColorSyncProfile!, CFString!) -> Bool

func ColorSyncProfileCopyData(ColorSyncProfile!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFData>!

func ColorSyncProfileCopyDescriptionString(ColorSyncProfile!) -> Unmanaged&lt;CFString>?

