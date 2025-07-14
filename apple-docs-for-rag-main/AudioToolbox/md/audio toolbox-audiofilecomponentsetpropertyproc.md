

- Audio Toolbox
-  AudioFileComponentSetPropertyProc 

Type Alias

# AudioFileComponentSetPropertyProc

macOS

``` source
typealias AudioFileComponentSetPropertyProc = (UnsafeMutableRawPointer, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus
```

## See Also

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentGetPropertyProc

Audio File Component Specific Properties

