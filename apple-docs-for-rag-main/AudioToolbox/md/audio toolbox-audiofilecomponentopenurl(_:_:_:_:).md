

- Audio Toolbox
-  AudioFileComponentOpenURL(\_:\_:\_:\_:) 

Function

# AudioFileComponentOpenURL(\_:\_:\_:\_:)

macOS 10.5+

``` source
func AudioFileComponentOpenURL(
    _ inComponent: AudioFileComponent,
    _ inFileRef: CFURL,
    _ inPermissions: Int8,
    _ inFileDescriptor: Int32
) -> OSStatus
```

## See Also

### Opening and Closing Audio Files

func AudioFileComponentCreateURL(AudioFileComponent, CFURL, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32) -> OSStatus

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

