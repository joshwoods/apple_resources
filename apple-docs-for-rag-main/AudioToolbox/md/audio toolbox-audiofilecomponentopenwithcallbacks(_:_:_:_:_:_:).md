

- Audio Toolbox
-  AudioFileComponentOpenWithCallbacks(\_:\_:\_:\_:\_:\_:) 

Function

# AudioFileComponentOpenWithCallbacks(\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func AudioFileComponentOpenWithCallbacks(
    _ inComponent: AudioFileComponent,
    _ inClientData: UnsafeMutableRawPointer,
    _ inReadFunc: AudioFile_ReadProc,
    _ inWriteFunc: AudioFile_WriteProc,
    _ inGetSizeFunc: AudioFile_GetSizeProc,
    _ inSetSizeFunc: AudioFile_SetSizeProc
) -> OSStatus
```

## See Also

### Opening and Closing Audio Files

func AudioFileComponentCreateURL(AudioFileComponent, CFURL, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

func AudioFileComponentOpenURL(AudioFileComponent, CFURL, Int8, Int32) -> OSStatus

func AudioFileComponentCloseFile(AudioFileComponent) -> OSStatus

func AudioFileComponentOptimize(AudioFileComponent) -> OSStatus

typealias AudioFileComponent

typealias AudioFileComponentPropertyID

typealias AudioFileComponentCreateURLProc

typealias AudioFileComponentOpenWithCallbacksProc

typealias AudioFileComponentOpenURLProc

typealias AudioFileComponentCloseProc

typealias AudioFileComponentOptimizeProc

