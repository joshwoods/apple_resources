

- Audio Toolbox
- Deprecated Symbols
-  Hardware Codec Capabilities 

API Collection

# Hardware Codec Capabilities

A constant to determine which hardware codecs can be used.

## Overview

Use this property to determine whether a desired set of codecs can be simultaneously instantiated.

Hardware-based codecs can be used only when playing or recording using Audio Queue Services or using interfaces, such as AVFoundation, which use Audio Queue Services. In particular, you cannot use hardware-based audio codecs with OpenAL or when using the I/O audio unit.

When describing the presence of a hardware codec, the system does not consider the current audio session category. Some categories disallow the use of hardware codecs. A set of hardware codecs is considered available, by this constant, based only on whether the hardware supports the specified combination of codecs.

Some codecs may be available in both hardware and software implementations. Use the kAudioFormatProperty_Encoders and kAudioFormatProperty_Decoders constants to determine whether a given codec is present, and whether it is hardware or software-based.

Software-based codecs can always be instantiated, so there is no need to use this constant when using software encoding or decoding.

The following code example illustrates how to check whether or not a hardware AAC encoder and a hardware AAC decoder are available, in that order of priority:

```
AudioClassDescription requestedCodecs[2] = {
    {
        kAudioEncoderComponentType,
        kAudioFormatAAC,
        kAppleHardwareAudioCodecManufacturer
    },
    {
        kAudioDecoderComponentType,
        kAudioFormatAAC,
        kAppleHardwareAudioCodecManufacturer
    }
};

UInt32 successfulCodecs = 0;
size = sizeof (successfulCodecs);
OSStatus result =   AudioFormatGetProperty (
                        kAudioFormatProperty_HardwareCodecCapabilities,
                        requestedCodecs,
                        sizeof (requestedCodecs),
                        &size,
                        &successfulCodecs
                    );
switch (successfulCodecs) {
    case 0:
        // aac hardware encoder is unavailable. aac hardware decoder availability
        // is unknown; could ask again for only aac hardware decoding
    case 1:
        // aac hardware encoder is available but, while using it, no hardware
        // decoder is available.
    case 2:
        // hardware encoder and decoder are available simultaneously
}
```

See also Audio Codec Component Constants and Audio Codec Manufacturer and Implementation Types.

## Topics

### Constants

var kAudioFormatProperty_HardwareCodecCapabilities: AudioFormatPropertyID

A `UInt32` value indicating the number of codecs from the specified list that can be used, if the application were to begin using them in the specified order. Set the `inSpecifier` parameter to an array of `AudioClassDescription` structures that describes a set of one or more audio codecs. If the property value is the same as the size of the array in the `inSpecifier` parameter, all of the specified codecs can be used.

## See Also

### Constants

Audio Unit Attenuation Properties

Audio Unit Instrument Errors

Anonymous

Anonymous

Audio Graph Errors

Audio Converter Property ID

Anonymous

Anonymous

Anonymous

Anonymous

Anonymous

Anonymous

Anonymous

Music Device Properties

3D Mixer Audio Unit Properties

Properties for the Apple 3D Mixer audio unit.

