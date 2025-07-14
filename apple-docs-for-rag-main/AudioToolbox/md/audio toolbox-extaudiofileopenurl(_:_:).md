

- Audio Toolbox
-  ExtAudioFileOpenURL(\_:\_:) 

Function

# ExtAudioFileOpenURL(\_:\_:)

Opens an existing audio file for reading, and associates it with a new extended audio file object.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileOpenURL(
    _ inURL: CFURL,
    _ outExtAudioFile: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inURL`  

The audio file to read.

`outExtAudioFile`  

On output, a newly allocated extended audio file object.

## Return Value

A result code.

## See Also

### Managing Extended Audio File Objects

func ExtAudioFileCreateWithURL(CFURL, AudioFileTypeID, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioChannelLayout>?, UInt32, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Creates a new audio file and associates it with a new extended audio file object.

func ExtAudioFileDispose(ExtAudioFileRef) -> OSStatus

Disposes of an extended audio file object and closes the associated file.

func ExtAudioFileWrapAudioFileID(AudioFileID, Bool, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Wraps an audio file object in an extended audio file object.

