

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Average video bit rate 

Article

# Average video bit rate

## Overview

Containing profile atom  
Track (video), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'avvb'`

`feature-value`  
Unsigned `int(32)` indicating average video bit rate in bits per second

## Feature Values

The value is an unsigned 32-bit integer indicating the average video bit rate in bits per second.

Example: 1 Mbps = 1000000.

## Writer Responsibilities

A writer of the average video bit rate feature should record a value that is equal to or greater than the average bit rate for the video track, measured across all media samples. A writer (such as a CE device) may choose to record a constant value so long as that value is greater than or equal to the average bit rate that may be encoded. It is also permitted to record a value set by the video encoder during initialization so long as the value equals or exceeds the average calculated from the resulting file.

## Feature Value Algorithm

Ideally, the long-term average: total sample sizes divided by total sample durations.

If the feature is written for a newly encoded track (as by a CE device), it is permitted to record a value used to initialize the video encoder. If the video track is edited and the average video bit rate recalculated, it may be calculated as an overall average based on the sample table.

## Reader Responsibilities

A reader of the average video bit rate feature value should compare the recorded value with its own limits to determine if the content can be played. The reader should not perform an equality comparison (=) but instead a relative comparison (\, or \>=).

Because a writer may record a larger value than the actual video bit rate, a reader should not interpret this as the actual video bit rate. To determine the current or actual bit rate, the reader may need to perform an inspection of the video track’s sample table.

## Comments

The value of this feature should be deducible from information found in the sample table. Track edits must be considered in its calculation. Note that for highly variable bit rate video, the average rate may not be a typical rate.

## See Also

### Setting features

Table of features

Maximum video bit rate

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

Video variable frame rate indication

