

- Audio Toolbox
-  AudioFileCreateWithURL(\_:\_:\_:\_:\_:) 

Function

# AudioFileCreateWithURL(\_:\_:\_:\_:\_:)

Creates a new audio file, or initializes an existing file, specified by a URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileCreateWithURL(
    _ inFileRef: CFURL,
    _ inFileType: AudioFileTypeID,
    _ inFormat: UnsafePointer,
    _ inFlags: AudioFileFlags,
    _ outAudioFile: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inFileRef`  

The fully specified path of the file to create or initialize.

`inFileType`  

The type of audio file to create. See AudioFileTypeID for constants that can be used.

`inFormat`  

A pointer to the structure that describes the format of the data.

`inFlags`  

Relevant flags for creating or opening the file. If eraseFile is set, it erases an existing file. If the flag is not set, the function fails fails if the URL is an existing file.

`outAudioFile`  

On output, a pointer to a newly created or initialized file.

## Return Value

A result code. See Result Codes.

## Discussion

This function uses a `CFURLRef` type rather than the `FSRef` type used by the deprecated AudioFileCreate function.

## See Also

### Creating and Initializing Audio Files

func AudioFileInitializeWithCallbacks(UnsafeMutableRawPointer, AudioFile_ReadProc, AudioFile_WriteProc, AudioFile_GetSizeProc, AudioFile_SetSizeProc, AudioFileTypeID, UnsafePointer&lt;AudioStreamBasicDescription>, AudioFileFlags, UnsafeMutablePointer&lt;AudioFileID?>) -> OSStatus

Deletes the content of an existing file and assigns callbacks to the audio file object.

