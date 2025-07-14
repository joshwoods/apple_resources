

- Audio Toolbox
-  AudioFileComponentGetGlobalInfoSizeProc 

Type Alias

# AudioFileComponentGetGlobalInfoSizeProc

macOS

``` source
typealias AudioFileComponentGetGlobalInfoSizeProc = (UnsafeMutableRawPointer, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer) -> OSStatus
```

## See Also

### Getting the Global Information

func AudioFileComponentGetGlobalInfo(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetGlobalInfoSize(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentGetGlobalInfoProc

