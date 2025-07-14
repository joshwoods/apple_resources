

- Audio Toolbox
-  AudioFileComponentInitializeWithCallbacks(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentInitializeWithCallbacks(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentInitializeWithCallbacks(
    _ inComponent: AudioFileComponent,
    _ inClientData: UnsafeMutableRawPointer,
    _ inReadFunc: AudioFile_ReadProc,
    _ inWriteFunc: AudioFile_WriteProc,
    _ inGetSizeFunc: AudioFile_GetSizeProc,
    _ inSetSizeFunc: AudioFile_SetSizeProc,
    _ inFileType: UInt32,
    _ inFormat: UnsafePointer,
    _ inFlags: UInt32
) -> OSStatus
```

## See Also

### Configuring the Callbacks

Audio File Component Selectors

typealias AudioFileComponentInitializeWithCallbacksProc

