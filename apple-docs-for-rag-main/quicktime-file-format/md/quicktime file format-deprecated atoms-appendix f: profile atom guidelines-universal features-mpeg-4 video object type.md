

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  MPEG-4 video object type 

Article

# MPEG-4 video object type

## Overview

Containing profile atom  
Track (video), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'m4vo'`

`feature-value`  
Unsigned `int(32)` where the least significant 8 bits hold the `video_object_type_indication` found in the `VideoObjectLayer` (Described in ISO/IEC 14496-2, subclause 6.2.3). The `VideoObjectLayer` is found in the MPEG-4 Elementary Stream Descriptor Atom within the `'esds'` sample description atom of the video sample description for the QuickTime video codec of type `'mp4v'`.

## Feature Values

The value is a video object type constant that indicates a set of video tools. The list of video object type constants is defined in specification ISO/IEC 14496-2, subclause 6.3.3. The least significant 8 bits hold the value. The most significant 24 bits should be set to `0`.

Example: The Simple Object Type video object is indicated by the value `1`.

## Writer Responsibilities

A writer of the MPEG-4 Video Object Type feature should record the 8 bits corresponding to the `video_object_type_indication` found in the `VideoObjectLayer` within the `ES_descriptor`’s video `DecoderSpecificConfig`. The most significant 24 bits of the value should be set to `0`. This feature should be written only for MPEG-4 video of video object type `1` (Video ID). If the MPEG-4 video does not use Video ID (`1`) for `visual_object_type`, the esds will have no `VideoObjectLayer` and consequently no `video_object_type_indication`. In this case, no MPEG-4 Video Object Type feature should be written.

Note

A writer that records the MPEG-4 Video Object Type feature for encoded video using the Video ID visual object type is encouraged to write the MPEG-4 Video Codec and MPEG-4 Video Profile features as well.

## Feature Value Algorithm

The MPEG-4 video object type is the least significant 8 bits of the `video_object_type_indication` found in the `VideoObjectLayer`. See ISO/IEC 14496-2, subclause 6.2.3. The `VideoObjectLayer` is found in the MPEG-4 Elementary Stream Descriptor Atom within the `'esds'` sample description atom of the video sample description for the QuickTime video codec of type `'mp4v'`.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with the set of MPEG-4 video tools supported by the reader.

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

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

