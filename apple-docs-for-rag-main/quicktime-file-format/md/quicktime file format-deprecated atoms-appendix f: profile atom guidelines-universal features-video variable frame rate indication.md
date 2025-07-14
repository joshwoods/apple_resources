

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Video variable frame rate indication 

Article

# Video variable frame rate indication

## Overview

Containing profile atom  
Track (video), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'vvfp'`

`feature-value`  
Unsigned `int(32)` holding the value `0` if the frame rate is constant or the value `1` if the frame durations vary

## Feature Values

The feature value holds one of the following two values: `0` if all video samples have the same display duration, or `1` if any video samples vary in duration.

## Writer Responsibilities

A writer of the Video Variable Frame Rate Indication feature should compare the video track sample durations. If all considered durations have the same value, the value `0` indicating constant frame rate should be recorded. If any durations differ, the value `1` should be recorded for the feature. No other value should be recorded.

## Feature Value Algorithm

If the Time to Sample table records a constant duration for all samples, then record `0`, else record `1`.

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

