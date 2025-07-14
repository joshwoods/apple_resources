

- Audio Toolbox
-  AudioFileOpenURL(\_:\_:\_:\_:) 

Function

# AudioFileOpenURL(\_:\_:\_:\_:)

Open an existing audio file specified by a URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileOpenURL(
    _ inFileRef: CFURL,
    _ inPermissions: AudioFilePermissions,
    _ inFileTypeHint: AudioFileTypeID,
    _ outAudioFile: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inFileRef`  

The URL of an existing audio file.

`inPermissions`  

The read-write permissions you want to assign to the file. Use the permission constants in AudioFilePermissions.

`inFileTypeHint`  

A hint for the file type of the designated file. For files without filename extensions and with types not easily or uniquely determined from the data (such as ADTS or AC3), use this hint to indicate the file type. Otherwise, pass `0`. Only use this hint in macOS versions 10.3.1 or greater. In all earlier versions, any attempt to open these files fails.

`outAudioFile`  

On output, a pointer to the newly opened audio file.

## Return Value

A result code. See Result Codes.

## See Also

### Opening and Closing Audio Files

func AudioFileOpenWithCallbacks(UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc?, AudioFile_GetSizeProc, AudioFile_SetSizeProc?, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileID?>) -> OSStatus

Opens an existing file with callbacks you provide.

func AudioFileClose(AudioFileID) -> OSStatus

Closes an audio file.

