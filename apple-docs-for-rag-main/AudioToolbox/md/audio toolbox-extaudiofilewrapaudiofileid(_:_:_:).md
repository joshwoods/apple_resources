

- Audio Toolbox
-  ExtAudioFileWrapAudioFileID(\_:\_:\_:) 

Function

# ExtAudioFileWrapAudioFileID(\_:\_:\_:)

Wraps an audio file object in an extended audio file object.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileWrapAudioFileID(
    _ inFileID: AudioFileID,
    _ inForWriting: Bool,
    _ outExtAudioFile: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inFileID`  

The audio file object to wrap.

`inForWriting`  

Use `true` if you intend to write to the audio file, `false` otherwise.

`outExtAudioFile`  

On output, a newly allocated extended audio file object.

## Return Value

A result code.

## Discussion

Allocates a new extended audio file object that wraps an existing audio file object. Your application is responsible for keeping the audio file object open until the extended audio file object is disposed.

## See Also

### Managing Extended Audio File Objects

func ExtAudioFileCreateWithURL(CFURL, AudioFileTypeID, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioChannelLayout>?, UInt32, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Creates a new audio file and associates it with a new extended audio file object.

func ExtAudioFileDispose(ExtAudioFileRef) -> OSStatus

Disposes of an extended audio file object and closes the associated file.

func ExtAudioFileOpenURL(CFURL, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Opens an existing audio file for reading, and associates it with a new extended audio file object.

