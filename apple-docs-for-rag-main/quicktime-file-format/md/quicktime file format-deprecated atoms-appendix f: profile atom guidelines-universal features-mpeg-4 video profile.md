

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  MPEG-4 video profile 

Article

# MPEG-4 video profile

## Overview

Containing profile atom  
Track (video), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
’`m4vp'`

`feature-value`  
Unsigned `int(32)` where least significant 8 bits hold the `profile_and_level_indication` from the `visual_object_sequence`, as defined in specification ISO/IEC 14496-2, retrieved from the video parameters for the MPEG-4 video codec description. The top 24 bits must be set to `0`.

## Feature Values

The least significant 8 bits hold the value. The most significant 24 bits of the feature value should be set to `0`.

## Writer Responsibilities

A writer of the MPEG-4 video profile feature should record the 8 bits corresponding to the `profile_and_level_indication` from the `visual_object_sequence`, as defined in specification ISO/IEC 14496-2, found in the video parameters encoded in the esds of the MPEG-4 video codec sample description (with QuickTime codec type `'mp4v'`).

Note

A writer that records the MPEG-4 video profile feature is encouraged also to write the QuickTime Video Codec Type feature.

## Feature Value Algorithm

The feature value is the `profile_and_level_indication` from the `visual_object_sequence`, as defined in specification ISO/IEC 14496-2, retrieved from the video parameters for the MPEG-4 video codec description.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with the set of profiles and levels supported by the reader.

## Comments

This feature may be present only if MPEG-4 video is used. Normally, the video codec type profile entry will also record that MPEG-4 video is present, unless no codec types are present (when, for example, an exhaustive list cannot be formed).

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

Average audio bit rate

QuickTime video codec type

QuickTime audio codec type

MPEG-4 video codec

MPEG-4 video object type

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

