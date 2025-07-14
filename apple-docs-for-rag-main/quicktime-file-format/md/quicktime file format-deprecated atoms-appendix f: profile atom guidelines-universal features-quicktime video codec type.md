

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  QuickTime video codec type 

Article

# QuickTime video codec type

## Overview

Containing profile atom  
Track (video), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'vfmt'`

`feature-value`  
Unsigned `int(32)` (a four-character-code) holding the QuickTime video codec type copied from the `ImageDescription` structure’s `cType` field

## Feature Values

This is the four-character-code found in a video sample description.

Examples: `'mp4v'`, `'jpeg'`.

## Writer Responsibilities

A writer of the QuickTime video codec type feature should record the four-character code corresponding to the QuickTime video format type or types also recorded in the video track’s sample descriptions.

Note

A writer that records the QuickTime Video Codec type for the `'mp4v'` codec is encouraged also to write the MPEG-4 Video Profile feature.

## Feature Value Algorithm

The feature value is the video codec type read from a QuickTime ImageDescription’s `cType` field. If there are multiple sample descriptions with different video codec types, multiple video codec type features should be recorded in the profile atom.

## Reader Responsibilities

A reader of this feature code should compare the recorded value by an equality comparison (using =) with the format codes supported by the reader.

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

Average audio bit rate

QuickTime audio codec type

MPEG-4 video profile

MPEG-4 video codec

MPEG-4 video object type

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

