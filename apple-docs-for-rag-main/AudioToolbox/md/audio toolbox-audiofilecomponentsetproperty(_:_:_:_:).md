

- Audio Toolbox
-  AudioFileComponentSetProperty(\_:\_:\_:\_:) 

Function

# AudioFileComponentSetProperty(\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentSetProperty(
    _ inComponent: AudioFileComponent,
    _ inPropertyID: AudioFileComponentPropertyID,
    _ inPropertyDataSize: UInt32,
    _ inPropertyData: UnsafeRawPointer
) -> OSStatus
```

## See Also

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentGetPropertyProc

typealias AudioFileComponentSetPropertyProc

Audio File Component Specific Properties

