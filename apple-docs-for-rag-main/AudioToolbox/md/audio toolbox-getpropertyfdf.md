

- Audio Toolbox
-  GetPropertyFDF 

Type Alias

# GetPropertyFDF

Mac CatalystmacOS

``` source
typealias GetPropertyFDF = (UnsafeMutableRawPointer, AudioFilePropertyID, UnsafeMutablePointer, UnsafeMutableRawPointer) -> OSStatus
```

## See Also

### Checking the File Format

func AudioFileComponentFileDataIsThisFormat(AudioFileComponent, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentExtensionIsThisFormat(AudioFileComponent, CFString, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentExtensionIsThisFormatProc

typealias AudioFileComponentFileDataIsThisFormatProc

typealias GetPropertyInfoFDF

