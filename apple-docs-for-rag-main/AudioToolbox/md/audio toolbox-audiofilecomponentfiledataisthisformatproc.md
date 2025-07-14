

- Audio Toolbox
-  AudioFileComponentFileDataIsThisFormatProc 

Type Alias

# AudioFileComponentFileDataIsThisFormatProc

macOS

``` source
typealias AudioFileComponentFileDataIsThisFormatProc = (UnsafeMutableRawPointer, UInt32, UnsafeRawPointer, UnsafeMutablePointer) -> OSStatus
```

## See Also

### Checking the File Format

func AudioFileComponentFileDataIsThisFormat(AudioFileComponent, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentExtensionIsThisFormat(AudioFileComponent, CFString, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentExtensionIsThisFormatProc

typealias GetPropertyFDF

typealias GetPropertyInfoFDF

