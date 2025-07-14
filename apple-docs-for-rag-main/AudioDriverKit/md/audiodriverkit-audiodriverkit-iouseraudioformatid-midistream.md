

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatID
-  MIDIStream 

Enumeration Case

# MIDIStream

A format for a stream of MIDI packet lists.

DriverKit 21.0+

``` source
MIDIStream
```

## Discussion

This format describes a stream of MIDIPacketList instances where the time stamps in the MIDIPacketList are sample offsets in the stream. The mSampleRate field describes how the stream passes time. This allows an Audio Unit that receives or generates this stream to define the time for any MIDI event within this list. It does so by using the sample rate, the number of frames it renders and the sample offsets within the MIDIPacketList.

This format uses no flags.

## See Also

### Non-Sample Formats

ParameterValueStream

A format for a side-chain of 32-bit floating-point data.

TimeCode

A format for a stream of time stamps.

