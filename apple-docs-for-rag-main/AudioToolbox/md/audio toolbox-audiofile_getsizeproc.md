

- Audio Toolbox
-  AudioFile_GetSizeProc 

Type Alias

# AudioFile_GetSizeProc

Gets file data size.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioFile_GetSizeProc = (UnsafeMutableRawPointer) -> Int64
```

## Parameters 

`inClientData`  

A pointer to the client data as set in the `inClientData` parameter to the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:) functions.

## Return Value

The callback should return the size of the data.

## Discussion

If you named your function `MyAudioFile_GetSizeProc`, you would declare it like this:

### Discussion

This callback gets invoked by an audio file object when it needs to get audio file data size. You pass this callback as a parameter when calling the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) and AudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:) functions.

## See Also

### Callbacks

typealias AudioFile_ReadProc

Reads audio data when used in conjunction with the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileInitializeWithCallbacks(_:_:_:_:_:_:_:_:_:) functions.)

typealias AudioFile_WriteProc

A callback for writing file data when used in conjunction with the AudioFileOpenWithCallbacks(_:_:_:_:_:_:_:) or AudioFileCreateWithURL(_:_:_:_:_:) functions.

typealias AudioFile_SetSizeProc

Sets file data size.

