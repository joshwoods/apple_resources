

- Audio Toolbox
-  Audio File Components 

API Collection

# Audio File Components

Get information about audio file formats, and about files containing audio data.

## Topics

### Opening and Closing Audio Files

func AudioFileComponentCreateURL(AudioFileComponent, CFURL, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

func AudioFileComponentOpenURL(AudioFileComponent, CFURL, Int8, Int32) -> OSStatus

func AudioFileComponentOpenWithCallbacks(AudioFileComponent, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc) -> OSStatus

func AudioFileComponentCloseFile(AudioFileComponent) -> OSStatus

func AudioFileComponentOptimize(AudioFileComponent) -> OSStatus

typealias AudioFileComponent

typealias AudioFileComponentPropertyID

typealias AudioFileComponentCreateURLProc

typealias AudioFileComponentOpenWithCallbacksProc

typealias AudioFileComponentOpenURLProc

typealias AudioFileComponentCloseProc

typealias AudioFileComponentOptimizeProc

### Configuring the Callbacks

func AudioFileComponentInitializeWithCallbacks(AudioFileComponent, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc, UInt32, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

Audio File Component Selectors

typealias AudioFileComponentInitializeWithCallbacksProc

### Getting the Global Information

func AudioFileComponentGetGlobalInfo(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetGlobalInfoSize(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer?, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentGetGlobalInfoProc

typealias AudioFileComponentGetGlobalInfoSizeProc

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

typealias AudioFileComponentSetUserDataProc

typealias CountUserDataFDF

typealias GetUserDataFDF

typealias GetUserDataSizeFDF

### Accessing Properties

func AudioFileComponentGetProperty(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentGetPropertyInfo(AudioFileComponent, AudioFileComponentPropertyID, UnsafeMutablePointer&lt;UInt32>?, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

func AudioFileComponentSetProperty(AudioFileComponent, AudioFileComponentPropertyID, UInt32, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentGetPropertyInfoProc

typealias AudioFileComponentGetPropertyProc

typealias AudioFileComponentSetPropertyProc

Audio File Component Specific Properties

### Reading and Writing Data

func AudioFileComponentReadBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPacketData(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentReadPackets(AudioFileComponent, Bool, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

func AudioFileComponentWriteBytes(AudioFileComponent, Bool, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

func AudioFileComponentWritePackets(AudioFileComponent, Bool, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeRawPointer) -> OSStatus

typealias AudioFileComponentReadBytesProc

typealias AudioFileComponentReadPacketDataProc

typealias AudioFileComponentReadPacketsProc

typealias AudioFileComponentWriteBytesProc

typealias AudioFileComponentWritePacketsProc

### Checking the File Format

func AudioFileComponentFileDataIsThisFormat(AudioFileComponent, UInt32, UnsafeRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioFileComponentExtensionIsThisFormat(AudioFileComponent, CFString, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

typealias AudioFileComponentExtensionIsThisFormatProc

typealias AudioFileComponentFileDataIsThisFormatProc

typealias GetPropertyFDF

typealias GetPropertyInfoFDF

## See Also

### Audio Files and Formats

Audio Format Services

Access information about audio formats and codecs.

Audio File Services

Read or write a variety of audio data to or from disk or a memory buffer.

Extended Audio File Services

Read and write compressed files and linear PCM audio files using a simplified interface.

Audio File Stream Services

Parse streamed audio files as the data arrives on the user’s computer.

Core Audio File Format

Parse the structure of Core Audio files.

