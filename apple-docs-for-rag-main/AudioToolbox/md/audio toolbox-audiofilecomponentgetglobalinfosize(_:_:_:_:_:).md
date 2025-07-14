

- Audio Toolbox
-  AudioFileComponentGetGlobalInfoSize(\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentGetGlobalInfoSize(\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentGetGlobalInfoSize(
    _ inComponent: AudioFileComponent,
    _ inPropertyID: AudioFileComponentPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ outPropertySize: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Getting the Global Information

func AudioFileComponentGetGlobalInfo(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

typealias AudioFileComponentGetGlobalInfoProc

typealias AudioFileComponentGetGlobalInfoSizeProc

