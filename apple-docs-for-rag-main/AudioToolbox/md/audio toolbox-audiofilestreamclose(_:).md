

- Audio Toolbox
-  AudioFileStreamClose(\_:) 

Function

# AudioFileStreamClose(\_:)

Closes and deallocates the specified audio file stream parser.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileStreamClose(_ inAudioFileStream: AudioFileStreamID) -> OSStatus
```

## Parameters 

`inAudioFileStream`  

The ID of the parser you wish to close. The parser ID is returned by the AudioFileStreamOpen(_:_:_:_:_:) function.

## Return Value

A result code. See Result Codes.

## See Also

### Related Documentation

func AudioFileStreamOpen(UnsafeMutableRawPointer?, AudioFileStream_PropertyListenerProc, AudioFileStream_PacketsProc, AudioFileTypeID, UnsafeMutablePointer&lt;AudioFileStreamID?>) -> OSStatus

Creates and opens a new audio file stream parser.

