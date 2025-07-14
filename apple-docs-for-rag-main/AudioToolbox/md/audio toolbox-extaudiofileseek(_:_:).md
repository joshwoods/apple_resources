

- Audio Toolbox
-  ExtAudioFileSeek(\_:\_:) 

Function

# ExtAudioFileSeek(\_:\_:)

Seeks to a specified frame in a file.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileSeek(
    _ inExtAudioFile: ExtAudioFileRef,
    _ inFrameOffset: Int64
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object that represents the file you are working with.

`inFrameOffset`  

The desired seek position, in sample frames, relative to the beginning of the file. Seek position is specified in the sample rate and frame count of the file’s audio data format—not your application’s audio data format.

## Return Value

A result code.

## Discussion

Sets the file’s read position to the specified sample frame number. A subsequent call to the ExtAudioFileRead(_:_:_:) function returns samples from precisely this location, even if it is located in the middle of a packet.

Ensure that the file you are seeking in is open for reading only. This function’s behavior with files open for writing is undefined.

## See Also

### Reading and Writing Audio Data

func ExtAudioFileRead(ExtAudioFileRef, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential read operation on an audio file.

func ExtAudioFileTell(ExtAudioFileRef, UnsafeMutablePointer&lt;Int64>) -> OSStatus

Gets an audio file’s read/write position.

func ExtAudioFileWrite(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential write operation on an audio file.

func ExtAudioFileWriteAsync(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>?) -> OSStatus

Perform an asynchronous, sequential write operation on an audio file.

