

- Core Audio Types
-  Audio Format Identifiers 

API Collection

# Audio Format Identifiers

Identifiers for supported audio formats.

## Overview

Use these identifiers to test for the presence of audio codecs on a system. If a given codec is present, you can use its identifier to specify that codec for data encoding or decoding, according to the capabilities of the codec. For more information, see Core Audio.

## Topics

### Format identifiers

var kAudioFormat60958AC3: AudioFormatID

A key that specifies the AC-3 codec, which provides data packaged for transport over an IEC 60958-compliant digital audio interface, and uses standard flags.

var kAudioFormatAC3: AudioFormatID

A key that specifies the AC-3 codec, and uses no flags.

var kAudioFormatAES3: AudioFormatID

A key that specifies the codec defined by the AES3-2003 standard, and uses no flags.

var kAudioFormatALaw: AudioFormatID

A key that specifies the A-law 2:1 codec, and uses no flags.

var kAudioFormatAMR: AudioFormatID

A key that specifies the Adaptive Multi-Rate (AMR) narrow band speech codec, and uses no flags.

var kAudioFormatAMR_WB: AudioFormatID

A key that specifies the AMR Wideband speech codec, and uses no flags.

var kAudioFormatAppleIMA4: AudioFormatID

A key that specifies Apple’s implementation of the IMA 4:1 ADPCM codec, and uses no flags.

var kAudioFormatAppleLossless: AudioFormatID

A key that specifies the Apple Lossless codec, and uses flags to indicate the bit depth of the source material.

var kAudioFormatAudible: AudioFormatID

A key that specifies the codec for Audible audio books, and uses no flags.

var kAudioFormatDVIIntelIMA: AudioFormatID

A key that specifies the codec defined by DVI/Intel IMA ADPCM - ACM code 17, and uses no flags.

var kAudioFormatEnhancedAC3: AudioFormatID

A key that specifies the Enhanced AC-3 codec, and uses no flags.

var kAudioFormatFLAC: AudioFormatID

A key that specifies the Free Lossless Audio Codec (FLAC), and uses flags to indicate the bit depth of the source material.

var kAudioFormatLinearPCM: AudioFormatID

A key that specifies the linear PCM codec, and uses the standard flags.

var kAudioFormatMACE3: AudioFormatID

A key that specifies the MACE 3:1 codec, and uses no flags.

var kAudioFormatMACE6: AudioFormatID

A key that specifies the MACE C:1 codec, and uses no flags.

var kAudioFormatMIDIStream: AudioFormatID

A key that specifies the MIDI stream codec, and uses no flags.

var kAudioFormatMPEG4AAC: AudioFormatID

A key that specifies the MPEG-4 AAC Low Complexity codec, and uses no flags.

var kAudioFormatMPEG4AAC_ELD: AudioFormatID

A key that specifies the MPEG-4 Enhanced Low Delay AAC codec, and uses no flags.

var kAudioFormatMPEG4AAC_ELD_SBR: AudioFormatID

A key that specifies the MPEG-4 Enhanced Low Delay AAC codec with a spectral band replication (SBR) extension layer, and uses no flags.

var kAudioFormatMPEG4AAC_ELD_V2: AudioFormatID

A key that specifies the MPEG-4 Enhanced Low Delay AAC version 2 codec, and uses no flags.

var kAudioFormatMPEG4AAC_HE: AudioFormatID

A key that specifies the MPEG-4 High-Efficiency AAC codec, and uses no flags.

var kAudioFormatMPEG4AAC_HE_V2: AudioFormatID

A key that specifies the MPEG-4 High-Efficiency AAC version 2 codec, and uses no flags.

var kAudioFormatMPEG4AAC_LD: AudioFormatID

A key that specifies the MPEG-4 Low Delay AAC codec, and uses no flags.

var kAudioFormatMPEG4AAC_Spatial: AudioFormatID

A key that specifies the MPEG-4 Spatial Audio Coding codec, and uses no flags.

var kAudioFormatMPEG4CELP: AudioFormatID

A key that specifies the MPEG-4 CELP codec, and uses flags to indicate the specific kind of data.

var kAudioFormatMPEG4HVXC: AudioFormatID

A key that specifies the MPEG-4 HVXC codec, and uses no flags.

var kAudioFormatMPEG4TwinVQ: AudioFormatID

A key that specifies the MPEG-4 TwinVQ codec, and uses no flags.

var kAudioFormatMPEGD_USAC: AudioFormatID

A key that specifies the MPEG-D Unified Speech and Audio Coding codec, and uses no flags.

var kAudioFormatMPEGLayer1: AudioFormatID

A key that specifies the MPEG-1/2, Layer I audio codec, and uses no flags.

var kAudioFormatMPEGLayer2: AudioFormatID

A key that specifies the MPEG-1/2, Layer II audio codec, and uses no flags.

var kAudioFormatMPEGLayer3: AudioFormatID

A key that specifies the MPEG-1/2, Layer III audio codec, and uses no flags.

var kAudioFormatMicrosoftGSM: AudioFormatID

A key that specifies the Microsoft GSM 6.10 - ACM code 49 codec, and uses no flags.

var kAudioFormatOpus: AudioFormatID

A key that specifies the Opus codec, and uses no flags.

var kAudioFormatParameterValueStream: AudioFormatID

A key that specifies the A side-chain of float 32 data that an audio unit provides for sending high-density parameter value control information, and uses no flags.

var kAudioFormatQDesign: AudioFormatID

A key that specifies the QDesign music codec, and uses no flags.

var kAudioFormatQDesign2: AudioFormatID

A key that specifies the QDesign 2 music codec, and uses no flags.

var kAudioFormatQUALCOMM: AudioFormatID

A key that specifies the Qualcomm PureVoice codec, and uses no flags.

var kAudioFormatTimeCode: AudioFormatID

A key that specifies the A stream of audio timestamp structures, and uses audio timestamp flags.

var kAudioFormatULaw: AudioFormatID

A key that specifies the μ-Law 2:1 codec, and uses no flags.

var kAudioFormatiLBC: AudioFormatID

A key that specifies the internet Low Bitrate Codec (iLBC) narrow band speech codec, and uses no flags.

## See Also

### Streams

struct AudioStreamBasicDescription

A format specification for an audio stream.

struct AudioStreamPacketDescription

A value that describes a packet in a buffer of audio data.

typealias AudioFormatFlags

A type definition for audio format flags.

Audio Format Flags

Commonly used combinations of data format flags for an audio stream description.

typealias AudioFormatID

A type definition for audio format identifiers.

let kAudioStreamAnyRate: Float64

A value that indicates that an audio stream can use any sample rate.

enum MPEG4ObjectID

Constants that define the type of MPEG-4 audio data.

Deprecated

