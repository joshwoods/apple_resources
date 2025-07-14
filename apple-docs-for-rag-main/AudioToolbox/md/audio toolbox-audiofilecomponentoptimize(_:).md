

- Audio Toolbox
-  AudioFileComponentOptimize(\_:) 

Function

# AudioFileComponentOptimize(\_:)

macOS 10.4+

``` source
func AudioFileComponentOptimize(_ inComponent: AudioFileComponent) -> OSStatus
```

## See Also

### Opening and Closing Audio Files

func AudioFileComponentCreateURL(AudioFileComponent, CFURL, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

func AudioFileComponentOpenURL(AudioFileComponent, CFURL, Int8, Int32) -> OSStatus

func AudioFileComponentOpenWithCallbacks(AudioFileComponent, UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc) -> OSStatus

func AudioFileComponentCloseFile(AudioFileComponent) -> OSStatus

typealias AudioFileComponent

typealias AudioFileComponentPropertyID

typealias AudioFileComponentCreateURLProc

typealias AudioFileComponentOpenWithCallbacksProc

typealias AudioFileComponentOpenURLProc

typealias AudioFileComponentCloseProc

typealias AudioFileComponentOptimizeProc

