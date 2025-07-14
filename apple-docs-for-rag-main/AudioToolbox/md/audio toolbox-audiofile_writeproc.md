

- Audio Toolbox
-  AudioFile_WriteProc 

Type Alias

# AudioFile_WriteProc

A callback for writing file data when used in conjunction with the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileCreateWithURL(_:_:_:_:_:) functions.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioFile_WriteProc = (UnsafeMutableRawPointer, Int64, UInt32, UnsafeRawPointer, UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`inClientData`  

A pointer to the client data as set in the `inClientData` parameter to AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) orAudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:).

`inPosition`  

An offset into the data from which to read.

`requestCount`  

The number of bytes to write.

`buffer`  

A pointer to the buffer containing the data to write.

`actualCount`  

Upon completion, the callback should set this to a pointer to the number of bytes successfully written.

## Return Value

A result code. See Result Codes.

## Discussion

If you named your function `MyAudioFile_WriteProc`, you would declare it like this:

### Discussion

This callback function is invoked when Audio File Services needs to write data.

## See Also

### Callbacks

typealias AudioFile_ReadProc

Reads audio data when used in conjunction with the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:) functions.)

typealias AudioFile_GetSizeProc

Gets file data size.

typealias AudioFile_SetSizeProc

Sets file data size.

