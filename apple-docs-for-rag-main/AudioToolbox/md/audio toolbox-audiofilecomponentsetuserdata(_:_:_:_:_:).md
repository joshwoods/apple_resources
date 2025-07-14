

- Audio Toolbox
-  AudioFileComponentSetUserData(\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentSetUserData(\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentSetUserData(
    _ inComponent: AudioFileComponent,
    _ inUserDataID: UInt32,
    _ inIndex: UInt32,
    _ inUserDataSize: UInt32,
    _ inUserData: UnsafeRawPointer
) -> OSStatus
```

## See Also

### Accessing the User Data

func AudioFileComponentGetUserData(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentCountUserData(AudioFileComponent, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentGetUserDataSize(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentRemoveUserData(AudioFileComponent, UInt32, UInt32) -> OSStatus

typealias AudioFileComponentCountUserDataProc

typealias AudioFileComponentGetUserDataProc

typealias AudioFileComponentGetUserDataSizeProc

typealias AudioFileComponentRemoveUserDataProc

typealias AudioFileComponentSetUserDataProc

typealias CountUserDataFDF

typealias GetUserDataFDF

typealias GetUserDataSizeFDF

