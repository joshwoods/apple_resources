

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  MPEG-4 audio codec 

Article

# MPEG-4 audio codec

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'mp4a'`

`feature-value`  
Unsigned `int(32)` where least significant 5 bits hold the `AudioObjectType` as found in the `AudioSpecificInfo` (as defined in specification ISO/IEC 14496-3, subclause 1.6) found in the esds of the MPEG-4 audio codec (QuickTime type `'mp4a'`) sample description

## Feature Values

The least significant 5 bits hold the value. The most significant 27 bits of the feature value should be set to `0`.

The list of audio object type constants is defined in specification ISO/IEC 14496-3, subclause 1.5.1.1.

Examples: AAC LC is indicated by the value `2`, CELP is indicated by the value `8`.

## Writer Responsibilities

A writer of the MPEG-4 Audio Codec feature should record the 5 bits corresponding to the `AudioObjectType` found in the `ES_descriptor`’s audio `DecoderSpecificConfig`. The most significant 27 bits of the value should be set to `0`.

Note

A writer that records the MPEG-4 Audio Codec feature is encouraged also to write the QuickTime Audio Codec Type feature.

## Feature Value Algorithm

The MPEG-4 audio codec value is the 5 bits of the `AudioObjectType` found in the `AudioSpecificInfo` (a `DecoderSpecificInfo`). See specification ISO/IEC 14496, subclause 1.6. The `AudioSpecificInfo` is found in the MPEG-4 Elementary Stream Descriptor Atom within the `siDecompressionParam` atom of the audio sample description for the QuickTime audio codec of type `'mp4a'`.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with the set of MPEG-4 audio decoders supported by the reader.

## Comments

Because the QuickTime `'mp4a'` codec may implement multiple audio decoders defined in specification ISO/IEC 14496 in the future, this feature allows the reader to determine the specific audio decoder needed to interpret the audio bit stream. The MPEG-4 Audio Codec feature should be present only if the `'mp4a'` audio codec is used in a sound track.

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

Average audio bit rate

QuickTime video codec type

QuickTime audio codec type

MPEG-4 video profile

MPEG-4 video codec

MPEG-4 video object type

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

