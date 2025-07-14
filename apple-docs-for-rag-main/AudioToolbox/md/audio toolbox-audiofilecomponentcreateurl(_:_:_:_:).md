

- Audio Toolbox
-  AudioFileComponentCreateURL(\_:\_:\_:\_:) 

Function

# AudioFileComponentCreateURL(\_:\_:\_:\_:)

macOS 10.5+

``` source
func AudioFileComponentCreateURL(
    _ inComponent: AudioFileComponent,
    _ inFileRef: CFURL,
    _ inFormat: UnsafePointer,
    _ inFlags: UInt32
) -> OSStatus
```

## See Also

### Opening and Closing Audio Files

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

