

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Audio variable bit rate indication 

Article

# Audio variable bit rate indication

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'avbr'`

`feature-value`  
Unsigned `int(32)` holding the value `0` if the audio is constant bit rate or `1` if the audio is variable bit rate

## Feature Values

The feature value holds one of the following two values: `0` if the audio is constant bit rate, or `1` if the audio is variable bit rate.

## Writer Responsibilities

A writer of the Audio Variable Bit Rate Indication feature should determine if the audio frames are constant or variable bit rate in nature and record either `0` or `1`, respectively.

## Feature Value Algorithm

Consult the audio sample descriptions. If the `compressionID` field in the sample descriptions is `0` or `-1`, then the audio is constant bit rate. If the field is `-2`, then the same algorithm as for video applies: if all the samples have both constant duration and constant size, then the audio is constant bit rate; otherwise it is variable.

## Reader Responsibilities

A reader of this feature code should only expect the values `0` or `1`.

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

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

