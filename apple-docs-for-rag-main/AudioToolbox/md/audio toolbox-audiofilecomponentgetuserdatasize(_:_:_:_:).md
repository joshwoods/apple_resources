

- Audio Toolbox
-  AudioFileComponentGetUserDataSize(\_:\_:\_:\_:) 

Function

# AudioFileComponentGetUserDataSize(\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentGetUserDataSize(
    _ inComponent: AudioFileComponent,
    _ inUserDataID: UInt32,
    _ inIndex: UInt32,
    _ outUserDataSize: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Accessing the User Data

func AudioFileComponentGetUserData(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentSetUserData(AudioFileComponent, UInt32, UInt32, UInt32, UnsafeRawPointer) -> OSStatus

func AudioFileComponentCountUserData(AudioFileComponent, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentRemoveUserData(AudioFileComponent, UInt32, UInt32) -> OSStatus

typealias AudioFileComponentCountUserDataProc

typealias AudioFileComponentGetUserDataProc

typealias AudioFileComponentGetUserDataSizeProc

typealias AudioFileComponentRemoveUserDataProc

typealias AudioFileComponentSetUserDataProc

typealias CountUserDataFDF

typealias GetUserDataFDF

typealias GetUserDataSizeFDF

