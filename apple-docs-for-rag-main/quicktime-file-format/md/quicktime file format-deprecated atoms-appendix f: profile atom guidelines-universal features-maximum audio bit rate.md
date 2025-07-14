

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Maximum audio bit rate 

Article

# Maximum audio bit rate

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'mabr'`

`feature-value`  
Unsigned `int(32)` indicating maximum audio bit rate in bits per second

## Feature Values

The value is an unsigned 32-bit integer indicating the maximum audio bit rate in bits per second that must be supported to guarantee playback of the audio. The actual maximum bit rate may be smaller, so a reader should not display this as the current bit rate.

Example: 128 kbps = 128000.

## Writer Responsibilities

A writer of the maximum audio bit rate feature should record a value that is equal to or greater than the current bit rate for the sound track. While the value may exceed the actual maximum bit-rate, the writer should attempt to minimize any over-estimation.

While recording the precise bit rate is preferred, it is not required. A writer (such as a CE device) may choose instead to record a constant value so long as that value is greater than or equal to the bit rate that may be encoded. It is also permitted to record a value set by the audio encoder during initialization so long as the value is never exceeded.

## Feature Value Algorithm

Use a sliding average over 1 second calculated from the sample tables.

If the feature is written for a newly encoded track (as by a CE device), it is permitted to record a value used to initialize the audio encoder so long as the value is never exceeded.

If the sound track is edited, and the audio bit rate is not constant, the maximum audio bit rate must be recalculated. Note that editing can change the duration of media samples, resulting in non-constant bit rate audio even when the sound track is encoded using a constant bit rate encoder. Maximum bit rate may be calculated as a sliding average over 1 second, based on the sample table. This can be calculated in the following manner:

1.  For each sample, calculate the average 1-second bit rate; choose the shortest run of samples, including the candidate sample, that comprise 1 second or more of audio, then divide the total data size of those samples by their total duration.

2.  Choose the maximum value from the list of calculated 1-second averages.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with its own limits to determine if the content can be played. The reader should not perform an equality comparison (=) but instead a relative comparison (\, or \>=).

Because this value may be an over-estimate of the true maximum bit rate, the reader should not refuse to play a file on the basis of this value, although a warning may be appropriate. To determine the current or actual bit rate, the reader may need to perform an inspection of the video track’s sample table.

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

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

