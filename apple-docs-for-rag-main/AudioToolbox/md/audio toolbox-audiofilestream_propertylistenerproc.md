

- Audio Toolbox
-  AudioFileStream_PropertyListenerProc 

Type Alias

# AudioFileStream_PropertyListenerProc

Invoked by an audio file stream parser when it finds a property value in the audio file stream.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioFileStream_PropertyListenerProc = (UnsafeMutableRawPointer, AudioFileStreamID, AudioFileStreamPropertyID, UnsafeMutablePointer) -> Void
```

## Parameters 

`inClientData`  

The value you provided in the `inClientData` parameter when you called the AudioFileStreamOpen(_:_:_:_:_:)function.

`inAudioFileStream`  

The ID of the audio file stream parser that invoked the callback. The parser ID is returned by the AudioFileStreamOpen(_:_:_:_:_:) function.

`inPropertyID`  

The four-character ID of the property that the parser found in the audio file data stream. See Audio File Stream Properties for possible values.

`ioFlags`  

On input, if the `kAudioFileStreamPropertyFlag_PropertyIsCached` value is set, the parser is caching the property value. If not, on output you can set the `kAudioFileStreamPropertyFlag_CacheProperty` flag to cause the parser to cache the value. See Audio File Stream Flags.

## Discussion

If you named your function `MyAudioFileStream_PropertyListenerProc`, you would declare it like this:

### Discussion

When the parser calls your property listener, check the `ioFlags` value to see if the property value is being cached. If not, you can call the AudioFileStreamGetPropertyInfo(_:_:_:_:) and AudioFileStreamGetProperty(_:_:_:_:) functions to obtain the value of the property from inside the property listener, or you can set the `kAudioFileStreamPropertyFlag_CacheProperty` flag on return to cause the parser to cache the value.

In some cases when you call the AudioFileStreamGetProperty(_:_:_:_:) function from inside the property listener, because of boundaries in the input data, the parser returns the result code `“kAudioFileStreamError_DataUnavailable”` indicating the value is not yet available. When unavailable data is requested from within the property listener, the parser begins caching the property value and calls the property listener again when the property value is available. If the `kAudioFileStreamPropertyFlag_PropertyIsCached` flag is not set, this is your only opportunity to get the value of the property, as the data is disposed of when the property listener callback returns.

## See Also

### Callbacks

typealias AudioFileStream_PacketsProc

Invoked by an audio file stream parser when it finds audio data in the audio file stream.

