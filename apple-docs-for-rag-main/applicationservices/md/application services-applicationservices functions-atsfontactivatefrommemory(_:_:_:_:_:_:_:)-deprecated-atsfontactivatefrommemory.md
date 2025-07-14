

- Application Services
- ApplicationServices Functions
-  ATSFontActivateFromMemory(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# ATSFontActivateFromMemory(\_:\_:\_:\_:\_:\_:\_:)

Mac Catalyst 13.1–13.1Deprecated

``` source
func ATSFontActivateFromMemory(
    _ iData: LogicalAddress!,
    _ iLength: Int,
    _ iContext: ATSFontContext,
    _ iFormat: ATSFontFormat,
    _ iReserved: UnsafeMutableRawPointer!,
    _ iOptions: ATSOptionFlags,
    _ oContainer: UnsafeMutablePointer!
) -> OSStatus
```

