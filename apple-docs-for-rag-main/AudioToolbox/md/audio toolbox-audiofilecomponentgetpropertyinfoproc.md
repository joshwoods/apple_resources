

- Audio Toolbox
-  AudioFileComponentGetPropertyInfoProc 

Type Alias

# AudioFileComponentGetPropertyInfoProc

macOS

``` source
typealias AudioFileComponentGetPropertyInfoProc = (UnsafeMutableRawPointer, AudioFileComponentPropertyID, UnsafeMutablePointer?, UnsafeMutablePointer?) -> OSStatus
```

## See Also

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyProc

typealias AudioFileComponentSetPropertyProc

Audio File Component Specific Properties

