

- Audio Toolbox
-  AudioFileComponentInitializeWithCallbacksProc 

Type Alias

# AudioFileComponentInitializeWithCallbacksProc

macOS

``` source
typealias AudioFileComponentInitializeWithCallbacksProc = (UnsafeMutableRawPointer, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc, UInt32, UnsafePointer, UInt32) -> OSStatus
```

## See Also

### Configuring the Callbacks

func AudioFileComponentInitializeWithCallbacks(AudioFileComponent, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc, UInt32, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

Audio File Component Selectors

