

- Audio Toolbox
- Audio Codec
-  Bit Rate Control Mode Constants 

API Collection

# Bit Rate Control Mode Constants

Bit rate control modes to be used with `kAudioCodecPropertyBitRateControlMode`.

## Overview

These modes are applicable only to encoders that can produce variable packet sizes, such as AAC.

## Topics

### Constants

var kAudioCodecBitRateControlMode_Constant: UInt32

var kAudioCodecBitRateControlMode_LongTermAverage: UInt32

var kAudioCodecBitRateControlMode_Variable: UInt32

var kAudioCodecBitRateControlMode_VariableConstrained: UInt32

## See Also

### Enumerations

Output Status Constants

Status values returned from the AudioCodecProduceOutputPackets(_:_:_:_:_:_:) function.

Program Target Levels

Dynamic Range Control Modes

Global Codec Properties

These read-only properties disclose the capabilities of the codec and remain the same for all instances of the codec.

Instance Codec Properties

Properties that can be set or read on an instance of the audio codec.

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

