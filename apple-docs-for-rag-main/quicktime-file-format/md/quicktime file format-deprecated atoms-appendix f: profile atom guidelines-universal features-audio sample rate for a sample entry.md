

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Audio sample rate for a sample entry 

Article

# Audio sample rate for a sample entry

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'ausr'`

`feature-value`  
Unsigned `int(32)` holding the audio sample rate in units per second (for example, `44100` for 44.1 kHz)

## Feature Values

This feature value is an unsigned 32-bit integer holding the audio sample rate in units per seconds (cycles per second). The value should be rounded up to the nearest integer if it has a fractional portion.

Examples: 24 kHz = `24000`, 44.1 kHz = `44100`.

## Writer Responsibilities

A writer of the Audio Sample Rate feature should record the integer portion (rounded up if there is a fractional portion) of the audio sample rate found in a sound track’s `SoundDescription` structure.

If multiple audio sample rates are used in the movie, then either all must recorded in the profile atom, or none must be recorded.

## Feature Value Algorithm

This is the integer portion of the sample rate from a QuickTime audio sample description (rounded up if there is a fractional portion). If the sample rate is greater than 64 kHz, the integer portion can be recorded here.

If a sample rate has a fractional portion, the writer should round up to the nearest integer. So, the `22254.54545` value that may occur in QuickTime audio as a Fixed value represented as `0x56EE8BA3` can be recorded as `22255`.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with its own audio sample rate limits. If the reader only supports discrete values (such as `44100`), it can perform equality comparisons (`=`). If the reader supports ranges of audio sample rates (such as all rates less than or equal to `32000`), the reader can perform relative comparisons (``, or `>=`).

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

