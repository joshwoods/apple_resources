

- Audio Toolbox
-  GetPropertyInfoFDF 

Type Alias

# GetPropertyInfoFDF

Mac CatalystmacOS

``` source
typealias GetPropertyInfoFDF = (UnsafeMutableRawPointer, AudioFilePropertyID, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
```

## See Also

### Checking the File Format

func AudioFileComponentFileDataIsThisFormat(AudioFileComponent, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentExtensionIsThisFormat(AudioFileComponent, CFString, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentExtensionIsThisFormatProc

typealias AudioFileComponentFileDataIsThisFormatProc

typealias GetPropertyFDF

