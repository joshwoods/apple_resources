

- Audio Toolbox
-  AudioFileStream_PacketsProc 

Type Alias

# AudioFileStream_PacketsProc

Invoked by an audio file stream parser when it finds audio data in the audio file stream.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioFileStream_PacketsProc = (UnsafeMutableRawPointer, UInt32, UInt32, UnsafeRawPointer, UnsafeMutablePointer?) -> Void
```

## Parameters 

`inClientData`  

The value you provided in the `inClientData` parameter when you called the AudioFileStreamOpen(_:_:_:_:_:) function.

`inNumberBytes`  

The number of bytes of data in the `inInputData` buffer.

`inNumberPackets`  

The number of packets of audio data in the `inInputData` buffer.

`inInputData`  

The audio data.

`inPacketDescriptions`  

An array of audio file stream packet description structures describing the data. Audio file stream packet description structures are described in Core Audio Data Types.

## Discussion

If you named your function `MyAudioFileStream_PacketsProc`, you would declare it like this:

### Discussion

For constant-bit-rate (CBR) audio data, your callback is typically called with as much data as you passed to the AudioFileStreamParseBytes(_:_:_:_:) function. At times, however, only a single packet might be passed because of boundaries in the input data. For variable-bit-rate (VBR) audio data, your callback might be called several times for each time you called the AudioFileStreamParseBytes(_:_:_:_:) function.

## See Also

### Callbacks

typealias AudioFileStream_PropertyListenerProc

Invoked by an audio file stream parser when it finds a property value in the audio file stream.

