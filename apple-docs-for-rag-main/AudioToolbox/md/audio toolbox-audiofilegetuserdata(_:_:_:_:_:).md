

- Audio Toolbox
-  AudioFileGetUserData(\_:\_:\_:\_:\_:) 

Function

# AudioFileGetUserData(\_:\_:\_:\_:\_:)

Gets a chunk from an audio file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
func AudioFileGetUserData(
    _ inAudioFile: AudioFileID,
    _ inUserDataID: UInt32,
    _ inIndex: UInt32,
    _ ioUserDataSize: UnsafeMutablePointer,
    _ outUserData: UnsafeMutableRawPointer
) -> OSStatus
```

## Parameters 

`inAudioFile`  

The audio file whose chunk you want to get.

`inUserDataID`  

The four-character code of the designated chunk.

`inIndex`  

An index that specifies which chunk with the four-character code specified in the `inUserDataID` parameter you want to query.

`ioUserDataSize`  

On input, a pointer to the size of the buffer that contains the designated chunk. On output, a pointer to the size of bytes that the system copied to the buffer.

`outUserData`  

A pointer to a buffer in which to copy the chunk data.

## Return Value

A result code if there’s an error (see Result Codes) or `noErr` if the operation succeeds.

## See Also

### Working with User Data

func AudioFileCountUserData(AudioFileID, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the number of user data items with a specified ID in a file.

func AudioFileGetUserDataSize(AudioFileID, UInt32, UInt32, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets the size of a user data item in an audio file.

func AudioFileGetUserDataSize64(AudioFileID, UInt32, UInt32, UnsafeMutablePointer&lt;UInt64>) -> OSStatus

Gets the size of a user data item in an audio file.

func AudioFileGetUserDataAtOffset(AudioFileID, UInt32, UInt32, Int64, UnsafeMutablePointer&lt;UInt32>, UnsafeMutableRawPointer) -> OSStatus

Gets part of the data from a chunk in an audio file.

func AudioFileSetUserData(AudioFileID, UInt32, UInt32, UInt32, UnsafeRawPointer) -> OSStatus

Sets a user data item in an audio file.

func AudioFileRemoveUserData(AudioFileID, UInt32, UInt32) -> OSStatus

Removes a user data item from an audio file.

