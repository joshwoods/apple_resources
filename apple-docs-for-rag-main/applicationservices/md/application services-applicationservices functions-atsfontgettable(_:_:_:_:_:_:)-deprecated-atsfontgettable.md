

- Application Services
- ApplicationServices Functions
-  ATSFontGetTable(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# ATSFontGetTable(\_:\_:\_:\_:\_:\_:)

Mac Catalyst 13.1–13.1Deprecated

``` source
func ATSFontGetTable(
    _ iFont: ATSFontRef,
    _ iTag: FourCharCode,
    _ iOffset: ByteOffset,
    _ iBufferSize: Int,
    _ ioBuffer: UnsafeMutableRawPointer!,
    _ oSize: UnsafeMutablePointer!
) -> OSStatus
```

