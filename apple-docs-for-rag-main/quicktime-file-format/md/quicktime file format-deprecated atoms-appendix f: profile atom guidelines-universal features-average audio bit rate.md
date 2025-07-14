

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Average audio bit rate 

Article

# Average audio bit rate

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'avab'`

`feature-value`  
Unsigned `int(32)` indicating average audio bit rate in bits per second

## Feature Values

The value is an unsigned 32-bit integer indicating the average audio bit rate in bits per second.

Example: 128 kbps = 128000.

## Writer Responsibilities

A writer of the average audio bit rate feature should record a value that is equal to or greater than the average bit rate for the sound track, measured across all media samples. A writer (such as a CE device) may choose to record a constant value so long as that value is greater than or equal to the average bit rate that may be encoded. It is also permitted to record a value set by the audio encoder during initialization so long as the value is never exceeded on average.

## Feature Value Algorithm

Normally, the long-term average: total sample sizes divided by total sample durations.

If the feature is written for a newly encoded track (as by a CE device), it is permitted to record a value used to initialize the audio encoder. If the sound track is edited and the average video bit rate recalculated, it may be calculated as an overall average based on the sample table.

## Reader Responsibilities

A reader of the average audio bit rate feature value should compare the recorded value with its own limits to determine if the content can be played. The reader should not perform an equality comparison (=) but instead a relative comparison (\, or \>=).

## Comments

The value of this feature should be deducible from information found in the sample table. Track edits normally need not be considered in the calculation for constant bit rate audio, but must be considered for variable bit rate audio or when track or movie segments containing constant bit rate audio are edited to alter their duration.

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

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

Video variable frame rate indication

