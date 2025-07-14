

- Audio Toolbox
-  AudioFileComponentOpenWithCallbacksProc 

Type Alias

# AudioFileComponentOpenWithCallbacksProc

macOS

``` source
typealias AudioFileComponentOpenWithCallbacksProc = (UnsafeMutableRawPointer, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc) -> OSStatus
```

## See Also

### Opening and Closing Audio Files

func AudioFileComponentCreateURL(AudioFileComponent, CFURL, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

func AudioFileComponentOpenURL(AudioFileComponent, CFURL, Int8, Int32) -> OSStatus

func AudioFileComponentOpenWithCallbacks(AudioFileComponent, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc) -> OSStatus

func AudioFileComponentCloseFile(AudioFileComponent) -> OSStatus

func AudioFileComponentOptimize(AudioFileComponent) -> OSStatus

typealias AudioFileComponent

typealias AudioFileComponentPropertyID

typealias AudioFileComponentCreateURLProc

typealias AudioFileComponentOpenURLProc

typealias AudioFileComponentCloseProc

typealias AudioFileComponentOptimizeProc

