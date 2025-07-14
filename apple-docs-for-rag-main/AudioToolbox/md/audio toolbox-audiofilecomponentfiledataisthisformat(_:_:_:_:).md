

- Audio Toolbox
-  AudioFileComponentFileDataIsThisFormat(\_:\_:\_:\_:) 

Function

# AudioFileComponentFileDataIsThisFormat(\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentFileDataIsThisFormat(
    _ inComponent: AudioFileComponent,
    _ inDataByteSize: UInt32,
    _ inData: UnsafeRawPointer,
    _ outResult: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Checking the File Format

func AudioFileComponentExtensionIsThisFormat(AudioFileComponent, CFString, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentExtensionIsThisFormatProc

typealias AudioFileComponentFileDataIsThisFormatProc

typealias GetPropertyFDF

typealias GetPropertyInfoFDF

