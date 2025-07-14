

- Audio Toolbox
- Audio Codec
-  Global Codec Properties 

API Collection

# Global Codec Properties

These read-only properties disclose the capabilities of the codec and remain the same for all instances of the codec.

## Overview

These properties are used with the AudioCodecGetProperty(_:_:_:_:) function.

The values of these properties are independent of the codec’s internal state and cannot be changed. They can be read at any time the codec is open.

## Topics

### Constants

var kAudioCodecPropertyFormatCFString: AudioCodecPropertyID

var kAudioCodecPropertyManufacturerCFString: AudioCodecPropertyID

var kAudioCodecPropertyNameCFString: AudioCodecPropertyID

## See Also

### Enumerations

Output Status Constants

Status values returned from the AudioCodecProduceOutputPackets(_:_:_:_:_:_:) function.

Program Target Levels

Dynamic Range Control Modes

Bit Rate Control Mode Constants

Bit rate control modes to be used with `kAudioCodecPropertyBitRateControlMode`.

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

