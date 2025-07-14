

- Audio Toolbox
-  AudioFileComponentSetUserDataProc 

Type Alias

# AudioFileComponentSetUserDataProc

macOS

``` source
typealias AudioFileComponentSetUserDataProc = (UnsafeMutableRawPointer, UInt32, UInt32, UInt32, UnsafeRawPointer) -> OSStatus
```

## See Also

### Accessing the User Data

func AudioFileComponentGetUserData(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentSetUserData(AudioFileComponent, UInt32, UInt32, UInt32, UnsafeRawPointer) -> OSStatus

func AudioFileComponentCountUserData(AudioFileComponent, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentGetUserDataSize(AudioFileComponent, UInt32, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentRemoveUserData(AudioFileComponent, UInt32, UInt32) -> OSStatus

typealias AudioFileComponentCountUserDataProc

typealias AudioFileComponentGetUserDataProc

typealias AudioFileComponentGetUserDataSizeProc

typealias AudioFileComponentRemoveUserDataProc

typealias CountUserDataFDF

typealias GetUserDataFDF

typealias GetUserDataSizeFDF

