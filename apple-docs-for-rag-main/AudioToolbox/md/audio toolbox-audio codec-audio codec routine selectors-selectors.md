

- Audio Toolbox
- Audio Codec
-  Audio Codec Routine Selectors 

API Collection

# Audio Codec Routine Selectors

Selectors used by the Component Manager to call routines implemented by the codec and exposed to developers through the Audio Codec Services API. These selectors are for use by codec developers; if you are calling Audio Codec Services functions, you don’t need to use these constants.

## Topics

### Constants

var kAudioCodecAppendInputBufferListSelect: UInt32

var kAudioCodecAppendInputDataSelect: UInt32

var kAudioCodecGetPropertyInfoSelect: UInt32

var kAudioCodecGetPropertySelect: UInt32

var kAudioCodecInitializeSelect: UInt32

var kAudioCodecProduceOutputBufferListSelect: UInt32

var kAudioCodecProduceOutputDataSelect: UInt32

var kAudioCodecResetSelect: UInt32

var kAudioCodecSetPropertySelect: UInt32

var kAudioCodecUninitializeSelect: UInt32

## See Also

### Enumerations

Output Status Constants

Status values returned from the AudioCodecProduceOutputPackets(_:_:_:_:_:_:) function.

Program Target Levels

Dynamic Range Control Modes

Bit Rate Control Mode Constants

Bit rate control modes to be used with `kAudioCodecPropertyBitRateControlMode`.

Global Codec Properties

These read-only properties disclose the capabilities of the codec and remain the same for all instances of the codec.

Instance Codec Properties

Properties that can be set or read on an instance of the audio codec.

Audio Codec Priming Method Constants

Values used with `kAudioCodecPropertyPrimeMethod`.

Audio Codec Quality Constants

Sound quality settings to be used with the property `kAudioCodecPropertyQualitySetting`.

Audio Codec Delays

Audio Codec Delay Modes

Audio Codec Properties

Audio Codec Errors

