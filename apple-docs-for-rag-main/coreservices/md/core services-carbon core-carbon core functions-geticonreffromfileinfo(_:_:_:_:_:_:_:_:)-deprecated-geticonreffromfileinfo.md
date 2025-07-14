

- Core Services
- Carbon Core
- Carbon Core Functions
-  GetIconRefFromFileInfo(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# GetIconRefFromFileInfo(\_:\_:\_:\_:\_:\_:\_:\_:)

macOS 10.1–10.13Deprecated

``` source
func GetIconRefFromFileInfo(
    _ inRef: UnsafePointer!,
    _ inFileNameLength: Int,
    _ inFileName: UnsafePointer!,
    _ inWhichInfo: FSCatalogInfoBitmap,
    _ inCatalogInfo: UnsafePointer!,
    _ inUsageFlags: IconServicesUsageFlags,
    _ outIconRef: UnsafeMutablePointer!,
    _ outLabel: UnsafeMutablePointer!
) -> OSStatus
```

