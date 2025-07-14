

- Audio Toolbox
-  AudioFileComponentGetProperty(\_:\_:\_:\_:) 

Function

# AudioFileComponentGetProperty(\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentGetProperty(
    _ inComponent: AudioFileComponent,
    _ inPropertyID: AudioFileComponentPropertyID,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Accessing Properties

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentGetPropertyProc

typealias AudioFileComponentSetPropertyProc

Audio File Component Specific Properties

