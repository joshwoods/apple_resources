

- Audio Toolbox
-  AudioFileComponentGetPropertyProc 

Type Alias

# AudioFileComponentGetPropertyProc

macOS

``` source
typealias AudioFileComponentGetPropertyProc = (UnsafeMutableRawPointer, AudioFileComponentPropertyID, UnsafeMutablePointer, UnsafeMutableRawPointer) -> OSStatus
```

## See Also

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentSetPropertyProc

Audio File Component Specific Properties

