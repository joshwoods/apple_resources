

- AudioDriverKit
- AudioDriverKit
- IOUserAudioFormatID
-  ParameterValueStream 

Enumeration Case

# ParameterValueStream

A format for a side-chain of 32-bit floating-point data.

DriverKit 21.0+

``` source
ParameterValueStream
```

## Discussion

The data in this kind of stream flows to or from an Audio Unit to send a high density of parameter value control information. An Audio Unit typically runs a ParameterValueStream at the sample rate of the AudioUnit’s audio data. It can also use some integer divisor of this rate, such as a half or a third of the audio’s sample rate. The sample rate of the IOUserAudioStreamBasicDescription describes this relationship.

This format uses no flags.

## See Also

### Non-Sample Formats

MIDIStream

A format for a stream of MIDI packet lists.

TimeCode

A format for a stream of time stamps.

