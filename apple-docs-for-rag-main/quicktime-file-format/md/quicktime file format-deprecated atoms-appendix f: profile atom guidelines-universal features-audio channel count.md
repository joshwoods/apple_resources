

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Audio channel count 

Article

# Audio channel count

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'achc'`

`feature-value`  
Unsigned `int(32)` holding the number of audio channels

## Feature Values

The feature value is an unsigned 32-bit integer holding the number of audio channels encoded by a Sound Track in the movie. For monaural, the value would be `1`. For stereo, the value would be `2`. Note that the audio channel count is a standard field in the sound sample description.

## Writer Responsibilities

A writer of the Audio Channel Count feature should determine the number of audio channels encoded in the sound track or tracks of the movie.

## Feature Value Algorithm

Consult the audio sample descriptions.

## Reader Responsibilities

The reader should be prepared to either play the specified number of channels or to map the audio to the number of channels the reader supports (for example, mixing down stereo sound for a monaural speaker).

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

