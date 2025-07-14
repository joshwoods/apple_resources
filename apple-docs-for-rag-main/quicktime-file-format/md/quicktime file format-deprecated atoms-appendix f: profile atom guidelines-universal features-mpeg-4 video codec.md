

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  MPEG-4 video codec 

Article

# MPEG-4 video codec

## Overview

Containing profile atom  
Track (video), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'mp4v'`

`feature-value`  
Unsigned `int(32)` where the least significant 4 bits holds the v`isual_object_type` as found in the `VisualObject` (as defined in specification ISO/IEC 14496-2, subclause 6.2.2) found in the esds of the MPEG-4 video codec (QuickTime type `'mp4v'`) sample description

## Feature Values

The least significant 4 bits hold the value. The most significant 28 bits of the feature value should be set to `0`.

The list of visual object type constants is defined in specification ISO/IEC 14496-2, subclause 6.3.2.

Example: Video ID is indicated by the value `1`.

## Writer Responsibilities

A writer of the MPEG-4 Video Codec feature should record the 4 bits corresponding to the `visual_object_type` found in the `VisualObject` within the `ES_descriptor`’s video `DecoderSpecificConfig`. The most significant 28 bits of the value should be set to `0`.

Note

A writer that records the MPEG-4 Video Codec feature is encouraged also to write the QuickTime Video Codec Type feature.

## Feature Value Algorithm

The MPEG-4 video codec is the 4 bits of the `visual_object_type` found in the `VisualObject`. See ISO/IEC 14496-2, subclause 6.2.2. The VisualObject is found in the MPEG-4 Elementary Stream Descriptor Atom within the `'esds'` sample description atom of the video sample description for the QuickTime video codec of type `'mp4v'`.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with the set of MPEG-4 video decoders supported by the reader.

## Comments

Because the QuickTime `'mp4v'` codec may implement multiple video decoders defined in specification ISO/IEC 14496 in the future, this feature allows the reader to determine the specific video decoder needed to interpret the video bit-stream.

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

MPEG-4 video object type

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

