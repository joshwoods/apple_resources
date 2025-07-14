

- Audio Toolbox
-  AudioFileComponentGetUserData(\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentGetUserData(\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentGetUserData(
    _ inComponent: AudioFileComponent,
    _ inUserDataID: UInt32,
    _ inIndex: UInt32,
    _ ioUserDataSize: UnsafeMutablePointer,
    _ outUserData: UnsafeMutableRawPointer
) -> OSStatus
```

## See Also

### Accessing the User Data

func AudioFileComponentSetUserData(AudioFileComponent, UInt32, UInt32, UInt32, UnsafeRawPointer) -> OSStatus

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

