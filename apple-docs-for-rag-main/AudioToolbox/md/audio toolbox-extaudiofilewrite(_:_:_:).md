

- Audio Toolbox
-  ExtAudioFileWrite(\_:\_:\_:) 

Function

# ExtAudioFileWrite(\_:\_:\_:)

Performs a synchronous, sequential write operation on an audio file.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileWrite(
    _ inExtAudioFile: ExtAudioFileRef,
    _ inNumberFrames: UInt32,
    _ ioData: UnsafePointer
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object that represents the file to write to.

`inNumberFrames`  

The number of frames to write.

`ioData`  

The buffer(s) from which audio data is written to the file.

## Return Value

A result code.

## Discussion

If the extended audio file object has an application data format, then the object’s converter converts the data in the `ioData` parameter to the file data format.

## See Also

### Reading and Writing Audio Data

func ExtAudioFileRead(ExtAudioFileRef, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential read operation on an audio file.

func ExtAudioFileSeek(ExtAudioFileRef, Int64) -> OSStatus

Seeks to a specified frame in a file.

func ExtAudioFileTell(ExtAudioFileRef, UnsafeMutablePointer&lt;Int64>) -> OSStatus

Gets an audio file’s read/write position.

func ExtAudioFileWriteAsync(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>?) -> OSStatus

Perform an asynchronous, sequential write operation on an audio file.

