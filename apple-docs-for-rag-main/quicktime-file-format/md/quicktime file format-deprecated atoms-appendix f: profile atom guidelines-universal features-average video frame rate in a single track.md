

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Average video frame rate in a single track 

Article

# Average video frame rate in a single track

## Overview

Containing profile atom  
Track (video), movie

part-ID  
`0x20202020` (universal feature)

feature-code  
`'tafr'`

feature-value  
An unsigned fixed-point (16.16) number holding the average video frame rate

## Feature Values

This is an unsigned fixed-point (16.16) number holding the average video frame rate. The integer portion of the number can range from `0` to `65535`.

Examples: 25 fps = `0x00190000`; 24 fps = `0x00180000`; 29.97 = `0x001DF853` (close approximation of a 30000/1001 ratio). The value may be rounded up to the nearest integer.

When present in a movie-level profile, these atoms document the average video frame rate of each track in the movie.

## Writer Responsibilities

A writer of the Average Video Frame Rate feature should record a 16.16 fixed-point value that is equal to or greater than the average video frame rate. A writer (such as a CE device) may choose to record a constant for the feature based on its current recording mode, even if the actual frame rate is less.

A writer of a new video track (such as a CE device recorder) may set the average frame rate feature value to a value set during video encoder initialization, so long as this frame rate is not exceeded by the actual average, as determined by the feature value algorithm described below.

If the average calculated frame rate is fractional (such as 22.3 fps), a writer may choose to round the value up to the nearest integer value (such as 23.0 fps for 22.3 fps).

## Feature Value Algorithm

This feature value is calculated by dividing the the total number of frames (samples) by the duration of the track. It is permissible to omit the first and last frames from this calculation, as they may have significantly different duration than the average.

## Reader Responsibilities

A reader of this feature code should understand that each frame is a video sample with its own independent and explicit duration. While it is possible for all frames to have the same duration, it is equally possible for the duration of any frame to be radically different from any other. Therefore, the average frame rate may not always be meaningful information.

The reader should not interpret the value of this feature as the current frame rate. To determine the current frame rate, the reader should use the video track’s sample table.

## Comments

A writer may choose to round up any fractional value of the fixed-point number to the nearest 16-bit integer leaving the lower 16 bits of the Fixed value set to `0`. So, in the case of the 29.97 approximation of `0x001DF853`, the writer could round this up to `0x001E0000` (which equals 30).

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

Video variable frame rate indication

