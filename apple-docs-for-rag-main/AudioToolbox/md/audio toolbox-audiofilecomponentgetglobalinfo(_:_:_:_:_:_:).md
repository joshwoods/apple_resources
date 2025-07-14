

- Audio Toolbox
-  AudioFileComponentGetGlobalInfo(\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentGetGlobalInfo(\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentGetGlobalInfo(
    _ inComponent: AudioFileComponent,
    _ inPropertyID: AudioFileComponentPropertyID,
    _ inSpecifierSize: UInt32,
    _ inSpecifier: UnsafeRawPointer?,
    _ ioPropertyDataSize: UnsafeMutablePointer,
    _ outPropertyData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Getting the Global Information

func AudioFileComponentGetGlobalInfoSize(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentGetGlobalInfoProc

typealias AudioFileComponentGetGlobalInfoSizeProc

