

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioFormatID 

Enumeration

# IOUserAudioFormatID

An enumeration of four character codes used to identify distinct audio data formats.

DriverKit 21.0+

``` source
enum IOUserAudioFormatID : uint32_t;
```

## Discussion

Some audio formats require additional configurations as indicated by the mFormatFlags field of the IOUserAudioStreamBasicDescription.

## Topics

### Pulse Code Modulation Formats

LinearPCM

The linear Pulse-Code Modulation (PCM) format.

AppleIMA4

The Apple implementation of IMA 4:1 Adaptive Differential Pulse-Code Modulation (ADPCM) format.

DVIIntelIMA

The DVI/Intel IMA Adaptive Differential Pulse-Code Modulation (ADPCM) format.

### Narrowband Formats

ALaw

The aLaw 2:1 format.

ULaw

The µLaw 2:1 format.

MicrosoftGSM

The Microsoft GSM 6.10 format.

### AC-3 Formats

AC3

The AC-3 format.

AC360958

The AC-3 format, packaged for transport over an IEC 60958-compliant digital audio interface.

EnhancedAC3

The Enhanced AC-3 format.

### Apple Lossless Formats

AppleLossless

The Apple Lossless format.

### AMR Speech Formats

AMR

The AMR Narrow Band speech codec.

AMR_WB

The AMR Wide Band speech codec.

### MPEG-4 Formats

MPEG4AAC

The MPEG-4 Low Complexity AAC audio object format.

MPEG4AAC_HE

The MPEG-4 High Efficiency AAC audio object format.

MPEG4AAC_LD

The MPEG-4 AAC Low Delay audio object format.

MPEG4AAC_ELD

The MPEG-4 AAC Enhanced Low Delay audio object format.

MPEG4AAC_ELD_SBR

The MPEG-4 AAC Enhanced Low Delay audio object with SBR extension layer format.

MPEG4AAC_HE_V2

The MPEG-4 High Efficiency AAC Version 2 audio object format.

MPEG4AAC_ELD_V2

The MPEG-4 AAC Enhanced Low Delay Version 2 audio object format.

MPEG4AAC_Spatial

The MPEG-4 Spatial Audio audio object format.

MPEG4CELP

The MPEG-4 Code Excited Linear Prediction (CELP) audio object format.

MPEG4HVXC

The MPEG-4 Harmonic Vector eXcitation Coding (HVXC) audio object format.

MPEG4TwinVQ

MPEG-4 TwinVQ audio object format.

### Other MPEG Formats

MPEGLayer1

The MPEG-1/2, Layer 1 audio format.

MPEGLayer2

The MPEG-1/2, Layer 2 audio format.

MPEGLayer3

The MPEG-1/2, Layer 3 audio format.

MPEGD_USAC

The MPEG-D Unified Speech and Audio Coding format.

### Non-Sample Formats

MIDIStream

A format for a stream of MIDI packet lists.

ParameterValueStream

A format for a side-chain of 32-bit floating-point data.

TimeCode

A format for a stream of time stamps.

### MACE Formats

MACE3

The MACE 3:1 format.

MACE6

The MACE 6:1 format.

### QDesign Music Formats

QDesign

The QDesign music format.

QDesign2

The QDesign2 music format.

### Qualcomm Formats

QUALCOMM

The QUALCOMM PureVoice format.

### AES-3 Formats

AES3

The AES3-2003 format.

### Other Lossless Formats

FLAC

The Free Lossless Audio Codec format.

### Audiobook Formats

Audible

The Audible audiobooks format.

### Open-Source Formats

Opus

The Opus codec format.

iLBC

The internet Low Bitrate Codec (iLBC) narrowband speech format.

## See Also

### Identifying the Format

mFormatID

The audio format identifier indicating the general kind of data in the stream.

mFormatFlags

Audio format flags for the stream’s format.

IOUserAudioFormatFlags

Flag values that provide more information about the format used by an audio stream basic description.

