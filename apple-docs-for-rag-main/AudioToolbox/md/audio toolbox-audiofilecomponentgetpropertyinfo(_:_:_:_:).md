

- Audio Toolbox
-  AudioFileComponentGetPropertyInfo(\_:\_:\_:\_:) 

Function

# AudioFileComponentGetPropertyInfo(\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentGetPropertyInfo(
    _ inComponent: AudioFileComponent,
    _ inPropertyID: AudioFileComponentPropertyID,
    _ outPropertySize: UnsafeMutablePointer?,
    _ outWritable: UnsafeMutablePointer?
) -> OSStatus
```

## See Also

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentGetPropertyProc

typealias AudioFileComponentSetPropertyProc

Audio File Component Specific Properties

