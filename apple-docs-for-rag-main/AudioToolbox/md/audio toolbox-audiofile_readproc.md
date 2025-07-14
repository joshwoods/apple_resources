

- Audio Toolbox
-  AudioFile_ReadProc 

Type Alias

# AudioFile_ReadProc

Reads audio data when used in conjunction with the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:) functions.)

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioFile_ReadProc = (UnsafeMutableRawPointer, Int64, UInt32, UnsafeMutableRawPointer, UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`inClientData`  

A pointer to the client data as set in the `inClientData` parameter to AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:).

`inPosition`  

An offset into the data from which to read.

`requestCount`  

The number of bytes to read.

`buffer`  

A pointer to the buffer in which to put the data read.

`actualCount`  

On output, the callback should set this parameter to a pointer to the number of bytes successfully read.

## Return Value

A result code. See Result Codes.

## Discussion

If you named your function `MyAudioFile_ReadProc`, you would declare it like this:

### Discussion

This callback function is called when Audio File Services needs to read data.

## See Also

### Callbacks

typealias AudioFile_WriteProc

A callback for writing file data when used in conjunction with the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileCreateWithURL(_:_:_:_:_:) functions.

typealias AudioFile_GetSizeProc

Gets file data size.

typealias AudioFile_SetSizeProc

Sets file data size.

