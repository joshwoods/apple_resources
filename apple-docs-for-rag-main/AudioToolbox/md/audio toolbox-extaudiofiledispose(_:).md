

- Audio Toolbox
-  ExtAudioFileDispose(\_:) 

Function

# ExtAudioFileDispose(\_:)

Disposes of an extended audio file object and closes the associated file.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileDispose(_ inExtAudioFile: ExtAudioFileRef) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object to close.

## Return Value

A result code.

## See Also

### Managing Extended Audio File Objects

func ExtAudioFileCreateWithURL(CFURL, AudioFileTypeID, UnsafePointer&lt;AudioStreamBasicDescription>, UnsafePointer&lt;AudioChannelLayout>?, UInt32, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Creates a new audio file and associates it with a new extended audio file object.

func ExtAudioFileOpenURL(CFURL, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Opens an existing audio file for reading, and associates it with a new extended audio file object.

func ExtAudioFileWrapAudioFileID(AudioFileID, Bool, UnsafeMutablePointer&lt;ExtAudioFileRef?>) -> OSStatus

Wraps an audio file object in an extended audio file object.

