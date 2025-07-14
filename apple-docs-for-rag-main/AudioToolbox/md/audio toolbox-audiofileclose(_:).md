

- Audio Toolbox
-  AudioFileClose(\_:) 

Function

# AudioFileClose(\_:)

Closes an audio file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileClose(_ inAudioFile: AudioFileID) -> OSStatus
```

## Parameters 

`inAudioFile`  

The file you want to close.

## Return Value

A result code. See Result Codes.

## See Also

### Opening and Closing Audio Files

func AudioFileOpenURL(CFURL, AudioFilePermissions, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileID?>) -> OSStatus

Open an existing audio file specified by a URL.

func AudioFileOpenWithCallbacks(UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc?, AudioFile_GetSizeProc, AudioFile_SetSizeProc?, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileID?>) -> OSStatus

Opens an existing file with callbacks you provide.

