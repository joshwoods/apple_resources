

- Audio Toolbox
- Audio Codec
-  Instance Codec Properties 

API Collection

# Instance Codec Properties

Properties that can be set or read on an instance of the audio codec.

## Overview

These properties are used with the AudioCodecGetProperty(_:_:_:_:) and AudioCodecSetProperty(_:_:_:_:) functions.

These properties are dependent on the codec’s current state. A property may be read/write or read only, depending on the data format of the codec.

These properties may have different values depending on whether the codec is in the initialized state. You can set writable properties only when the codec is not initialized. All properties can be read at any time the codec is open.

## Topics

### Constants

var kAudioCodecPropertyAdjustLocalQuality: AudioCodecPropertyID

var kAudioCodecPropertyApplicableBitRateRange: AudioCodecPropertyID

var kAudioCodecPropertyApplicableInputSampleRates: AudioCodecPropertyID

var kAudioCodecPropertyApplicableOutputSampleRates: AudioCodecPropertyID

var kAudioCodecPropertyBitRateControlMode: AudioCodecPropertyID

var kAudioCodecPropertyCurrentInputChannelLayout: AudioCodecPropertyID

var kAudioCodecPropertyCurrentInputFormat: AudioCodecPropertyID

var kAudioCodecPropertyCurrentInputSampleRate: AudioCodecPropertyID

var kAudioCodecPropertyCurrentOutputChannelLayout: AudioCodecPropertyID

var kAudioCodecPropertyCurrentOutputFormat: AudioCodecPropertyID

var kAudioCodecPropertyCurrentOutputSampleRate: AudioCodecPropertyID

var kAudioCodecPropertyCurrentTargetBitRate: AudioCodecPropertyID

var kAudioCodecPropertyDelayMode: AudioCodecPropertyID

var kAudioCodecPropertyDynamicRangeControlMode: AudioCodecPropertyID

var kAudioCodecPropertyFormatList: AudioCodecPropertyID

var kAudioCodecPropertyHasVariablePacketByteSizes: AudioCodecPropertyID

var kAudioCodecPropertyInputBufferSize: AudioCodecPropertyID

var kAudioCodecPropertyIsInitialized: AudioCodecPropertyID

var kAudioCodecPropertyMagicCookie: AudioCodecPropertyID

var kAudioCodecPropertyMaximumPacketByteSize: AudioCodecPropertyID

var kAudioCodecPropertyPacketFrameSize: AudioCodecPropertyID

var kAudioCodecPropertyPacketSizeLimitForVBR: AudioCodecPropertyID

var kAudioCodecPropertyPaddedZeros: AudioCodecPropertyID

var kAudioCodecPropertyPrimeInfo: AudioCodecPropertyID

var kAudioCodecPropertyPrimeMethod: AudioCodecPropertyID

var kAudioCodecPropertyProgramTargetLevel: AudioCodecPropertyID

var kAudioCodecPropertyProgramTargetLevelConstant: AudioCodecPropertyID

var kAudioCodecPropertyQualitySetting: AudioCodecPropertyID

var kAudioCodecPropertyRecommendedBitRateRange: AudioCodecPropertyID

var kAudioCodecPropertySettings: AudioCodecPropertyID

var kAudioCodecPropertySoundQualityForVBR: AudioCodecPropertyID

var kAudioCodecPropertyUsedInputBufferSize: AudioCodecPropertyID

var kAudioCodecPropertyAdjustCompressionProfile: AudioCodecPropertyID

var kAudioCodecPropertyAdjustTargetLevel: AudioCodecPropertyID

var kAudioCodecPropertyAdjustTargetLevelConstant: AudioCodecPropertyID

var kAudioCodecPropertyBitRateForVBR: AudioCodecPropertyID

var kAudioCodecPropertyEmploysDependentPackets: AudioCodecPropertyID

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

Audio Codec Priming Method Constants

Values used with `kAudioCodecPropertyPrimeMethod`.

Audio Codec Quality Constants

Sound quality settings to be used with the property `kAudioCodecPropertyQualitySetting`.

Audio Codec Routine Selectors

Selectors used by the Component Manager to call routines implemented by the codec and exposed to developers through the Audio Codec Services API. These selectors are for use by codec developers; if you are calling Audio Codec Services functions, you don’t need to use these constants.

Audio Codec Delays

Audio Codec Delay Modes

Audio Codec Properties

Audio Codec Errors

