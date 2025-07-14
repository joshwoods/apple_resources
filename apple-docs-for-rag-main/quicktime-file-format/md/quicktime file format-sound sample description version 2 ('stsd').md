

- QuickTime File Format
-  Sound sample description version 2 ('stsd') 

Atom

# Sound sample description version 2 ('stsd')

An updated sound sample description that adds high resolution audio.

## Mentioned in 

QuickTime File Format change log

## Overview

QuickTime 7 introduced a new version of the sound sample description, version 2, which extends QuickTime capabilities to include high resolution audio with another expansion of the sound sample description structure. In QuickTime 7, the sound and audio facilities are based on the Core Audio framework facilities and the Sound Manager has been deprecated. In this version of the sound sample description, the format field is set to `‘lpcm’` for uncompressed data. For compressed data formats, the format field is set to the compression type code (normally `‘mp4a’`) and the compression specifics and other features of QuickTime 7 are supplied by extensions.

The version field is set to `2` for this version of the sound sample description structure.

The sound sample description v2 structure adds the following new fields, appending to the v1 structure and renaming the four fields added in v1 to help ensure backwards compatibility with older applications.

Important

The values contained in these fields have different meanings for compressed and uncompressed audio. The meaning may not be easily deducible from the field name and require reference to the appropriate sound sample description extensions to understand fully.

Some definitions for sound sample description version 2:

- LPCM Frame: one uncompressed sample in each of the channels (for instance, 44100Hz audio has 44100 LPCM frames per second, whether it is mono, stereo, 5.1, or other possible values). In other words, LPCM Frames divided by the `audioSampleRate` value is duration in seconds.

- Audio Packet: For compressed audio, an audio packet is the natural compressed access unit of that format. For uncompressed audio, an audio packet is simply one LPCM frame.

- Fields prefixed by `const`: Note the three sound sample description v2 fields whose names start with `const`. These fields are only nonzero if the value is a constant. A zero in each field implies that the value is variable. For example: AAC audio would have a zero in `constBytesPerAudioPacket` because AAC has variable sized audio packets. Codecs with variable duration audio packets set a zero in `constLPCMFramesPerAudioPacket`.

## LPCM flag values

The formatSpecificFlags field carries flags significant to the layout and formatting of audio streams defined in the Core Audio underpinnings for sound sample description v2. These are enumerated in the Apple QuickTime/CoreAudioFormat.h interface file and are subject to a fuller interpretation in the context of the AudioStreamBasicDescription data type. See the CoreAudio, “Core Audio Framework Reference” in the OS X Developer Library.

```
enum
{
    kAudioFormatFlagIsFloat                  = (1 

## Topics

### Data fields

Sample description size

A 32-bit integer indicating the number of bytes in the sample description.

Data format

A 32-bit integer indicating the format of the stored data.

Reserved

Six bytes.

Data reference index

A 16-bit integer that contains the index of the data reference to use to retrieve data associated with samples that use this sample description.

Version

A 16-bit integer that holds the sample description version.

Revision level

A 16-bit integer.

Vendor

A 32-bit integer.

always3

A 16-bit integer field.

always16

A 16-bit integer field.

alwaysMinus2

A 16-bit integer field.

always0

A 16-bit integer field.

always65536

A 32-bit integer field.

sizeOfStructOnly

A 32-bit integer field providing the offset to sound sample description structure’s extensions.

numAudioChannels

A 32-bit integer field set to the number of audio channels.

always7F000000

A 32-bit integer field.

constBitsPerChannel

A 32-bit integer field which is set only if constant and only for uncompressed audio.

formatSpecificFlags

A 32-bit integer field which carries LPCM flag values.

constBytesPerAudioPacket

A 32-bit unsigned integer set to the number of bytes per packet only if this value is constant.

constLPCMFramesPerAudioPacket

A 32-bit unsigned integer set to the number of PCM frames per packet only if this value is constant.

## See Also

### Using sample descriptions

Sound sample description version 0 ('stsd')

A sound sample description that supports only uncompressed audio in raw or twos-complement format.

Sound sample description version 1 ('stsd')

An extended sound sample description that supports compressed audio, and includes the ability to add atoms to the sound description.

