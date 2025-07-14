

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  QuickTime audio codec type 

Article

# QuickTime audio codec type

## Overview

Containing profile atom  
Track (sound), movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'afmt'`

`feature-value`  
Unsigned `int(32)` (a four-character-code) holding the QuickTime audio codec type copied from `SoundDescription` structure’s `dataFormat` field

## Feature Values

This is the four-character-code found in a sound sample description.

Examples: `'mp4a'`, `'twos'`.

## Writer Responsibilities

A writer of the QuickTime audio codec type feature should record the four-character-code corresponding to the QuickTime audio format type or types also recorded in the sound track’s sample descriptions.

Note

A writer that records the QuickTime Audio Codec type for the `'mp4a'` codec is encouraged also to write the MPEG-4 Audio Codec feature.

## Feature Value Algorithm

The feature value is the audio codec type read from a `SoundDescription` structure’s `dataFormat` field. If there are multiple sample descriptions with different audio codec types, either all QuickTime Audio Codec Type features must be recorded in the profile atom or none must be recorded.

## Reader Responsibilities

A reader of this feature code should compare the recorded value by an equality comparison (using =) with the format codes supported by the reader.

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

Average audio bit rate

QuickTime video codec type

MPEG-4 video profile

MPEG-4 video codec

MPEG-4 video object type

MPEG-4 audio codec

Maximum video size in a movie

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

