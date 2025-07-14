

- Audio Toolbox
-  ExtAudioFileTell(\_:\_:) 

Function

# ExtAudioFileTell(\_:\_:)

Gets an audio file’s read/write position.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileTell(
    _ inExtAudioFile: ExtAudioFileRef,
    _ outFrameOffset: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object that represents the file you are working with.

`outFrameOffset`  

On output, the file’s current read/write position in sample frames. Read/write position is specified in the sample rate and frame count of the file’s audio data format—not your application’s audio data format.

## Return Value

A result code.

## See Also

### Reading and Writing Audio Data

func ExtAudioFileRead(ExtAudioFileRef, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential read operation on an audio file.

func ExtAudioFileSeek(ExtAudioFileRef, Int64) -> OSStatus

Seeks to a specified frame in a file.

func ExtAudioFileWrite(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential write operation on an audio file.

func ExtAudioFileWriteAsync(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>?) -> OSStatus

Perform an asynchronous, sequential write operation on an audio file.

