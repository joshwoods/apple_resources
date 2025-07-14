

- Audio Toolbox
- Audio File Components
-  Audio File Component Selectors 

API Collection

# Audio File Component Selectors

## Topics

### Selectors

var kAudioFileCloseSelect: Int

var kAudioFileCountUserDataSelect: Int

var kAudioFileCreateSelect: Int

var kAudioFileCreateURLSelect: Int

var kAudioFileDataIsThisFormatSelect: Int

var kAudioFileExtensionIsThisFormatSelect: Int

var kAudioFileFileDataIsThisFormatSelect: Int

var kAudioFileFileIsThisFormatSelect: Int

var kAudioFileGetGlobalInfoSelect: Int

var kAudioFileGetGlobalInfoSizeSelect: Int

var kAudioFileGetPropertyInfoSelect: Int

var kAudioFileGetUserDataAtOffsetSelect: Int

var kAudioFileGetUserDataSize64Select: Int

var kAudioFileGetPropertySelect: Int

var kAudioFileGetUserDataSelect: Int

var kAudioFileGetUserDataSizeSelect: Int

var kAudioFileInitializeSelect: Int

var kAudioFileInitializeWithCallbacksSelect: Int

var kAudioFileOpenSelect: Int

var kAudioFileOpenURLSelect: Int

var kAudioFileOpenWithCallbacksSelect: Int

var kAudioFileOptimizeSelect: Int

var kAudioFileReadBytesSelect: Int

var kAudioFileReadPacketDataSelect: Int

var kAudioFileReadPacketsSelect: Int

var kAudioFileRemoveUserDataSelect: Int

var kAudioFileSetPropertySelect: Int

var kAudioFileSetUserDataSelect: Int

var kAudioFileWriteBytesSelect: Int

var kAudioFileWritePacketsSelect: Int

## See Also

### Configuring the Callbacks

func AudioFileComponentInitializeWithCallbacks(AudioFileComponent, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc, UInt32, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

typealias AudioFileComponentInitializeWithCallbacksProc

