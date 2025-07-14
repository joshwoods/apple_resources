

- Audio Toolbox
-  AudioFileComponentExtensionIsThisFormat(\_:\_:\_:) 

Function

# AudioFileComponentExtensionIsThisFormat(\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentExtensionIsThisFormat(
    _ inComponent: AudioFileComponent,
    _ inExtension: CFString,
    _ outResult: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Checking the File Format

func AudioFileComponentFileDataIsThisFormat(AudioFileComponent, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentExtensionIsThisFormatProc

typealias AudioFileComponentFileDataIsThisFormatProc

typealias GetPropertyFDF

typealias GetPropertyInfoFDF

