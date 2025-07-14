

- ColorSync
-  ColorSyncIterateInstalledProfilesWithOptions(\_:\_:\_:\_:\_:) 

Function

# ColorSyncIterateInstalledProfilesWithOptions(\_:\_:\_:\_:\_:)

Mac Catalyst 13.0+macOS 10.13+

``` source
func ColorSyncIterateInstalledProfilesWithOptions(
    _ callBack: ColorSyncProfileIterateCallback?,
    _ seed: UnsafeMutablePointer?,
    _ userInfo: UnsafeMutableRawPointer?,
    _ options: CFDictionary?,
    _ error: UnsafeMutablePointer?>?
)
```

## See Also

### Functions

func ColorSyncAPIVersion() -> UInt32

func ColorSyncCreateCodeFragment(CFArray!, CFDictionary!) -> Unmanaged&lt;CFTypeRef>!

func ColorSyncProfileIsHLGBased(ColorSyncProfile!) -> Bool

func ColorSyncProfileIsMatrixBased(ColorSyncProfile!) -> Bool

func ColorSyncProfileIsPQBased(ColorSyncProfile!) -> Bool

func ColorSyncProfileIsWideGamut(ColorSyncProfile!) -> Bool

func ColorSyncTransformGetProfileSequence(ColorSyncTransform!) -> Unmanaged&lt;CFArray>?

