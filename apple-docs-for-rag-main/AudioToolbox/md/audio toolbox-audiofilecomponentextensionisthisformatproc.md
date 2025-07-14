

- Audio Toolbox
-  AudioFileComponentExtensionIsThisFormatProc 

Type Alias

# AudioFileComponentExtensionIsThisFormatProc

macOS

``` source
typealias AudioFileComponentExtensionIsThisFormatProc = (UnsafeMutableRawPointer, CFString, UnsafeMutablePointer) -> OSStatus
```

## See Also

### Checking the File Format

func AudioFileComponentFileDataIsThisFormat(AudioFileComponent, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentExtensionIsThisFormat(AudioFileComponent, CFString, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentFileDataIsThisFormatProc

typealias GetPropertyFDF

typealias GetPropertyInfoFDF

