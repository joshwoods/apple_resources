

- Audio Toolbox
-  ExtAudioFileWriteAsync(\_:\_:\_:) 

Function

# ExtAudioFileWriteAsync(\_:\_:\_:)

Perform an asynchronous, sequential write operation on an audio file.

iOS 2.1+iPadOS 2.1+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func ExtAudioFileWriteAsync(
    _ inExtAudioFile: ExtAudioFileRef,
    _ inNumberFrames: UInt32,
    _ ioData: UnsafePointer?
) -> OSStatus
```

## Parameters 

`inExtAudioFile`  

The extended audio file object that represents the file you want to write to.

`inNumberFrames`  

The number of frames to write.

`ioData`  

The buffer(s) from which audio data is written to the file.

## Return Value

A result code.

## Discussion

Writes the provided buffer list to an internal ring buffer and notifies an internal thread to perform the write at a later time. The first time this function is called, allocations may be performed. You can call this function with `0` frames and a `NULL` buffer in a non-time-critical context to initialize the asynchronous mechanism. Once initialized, subsequent calls are very efficient and do not take locks. This technique may be used to write to a file from a realtime thread.

Your application must not mix synchronous and asynchronous writes to the same file.

Pending writes are not guaranteed to be flushed to disk until the ExtAudioFileDispose(_:) function is called.

Errors may occur after this call has returned. Such errors may be returned from subsequent calls to this function.

## See Also

### Reading and Writing Audio Data

func ExtAudioFileRead(ExtAudioFileRef, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential read operation on an audio file.

func ExtAudioFileSeek(ExtAudioFileRef, Int64) -> OSStatus

Seeks to a specified frame in a file.

func ExtAudioFileTell(ExtAudioFileRef, UnsafeMutablePointer&lt;Int64>) -> OSStatus

Gets an audio file’s read/write position.

func ExtAudioFileWrite(ExtAudioFileRef, UInt32, UnsafePointer&lt;AudioBufferList>) -> OSStatus

Performs a synchronous, sequential write operation on an audio file.

