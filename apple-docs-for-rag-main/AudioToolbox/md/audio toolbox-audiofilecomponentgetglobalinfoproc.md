

- Audio Toolbox
-  AudioFileComponentGetGlobalInfoProc 

Type Alias

# AudioFileComponentGetGlobalInfoProc

macOS

``` source
typealias AudioFileComponentGetGlobalInfoProc = (UnsafeMutableRawPointer, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer, UnsafeMutableRawPointer) -> OSStatus
```

## See Also

### Getting the Global Information

func AudioFileComponentGetGlobalInfo(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetGlobalInfoSize(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentGetGlobalInfoSizeProc

