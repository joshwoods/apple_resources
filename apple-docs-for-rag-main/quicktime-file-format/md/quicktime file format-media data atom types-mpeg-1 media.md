

- QuickTime File Format
- Media data atom types
-  MPEG-1 media 

Article

# MPEG-1 media

Store MPEG-1 video streams, MPEG-1, layer 2 audio streams, and multiplexed MPEG-1 audio and video streams in QuickTime movies.

## Overview

MPEG-1 media is used to store MPEG-1 video streams, MPEG-1, layer 2 audio streams, and multiplexed MPEG-1 audio and video streams in QuickTime movies. It has a media type of `'MPEG'`.

## MPEG-1 Sample Description

The MPEG-1 sample description uses the standard sample description header, as described in Sample description atom ('stsd').

The data format field in the sample description is always set to `'MPEG'`. The MPEG-1 media handler adds no additional fields to the sample description.

Note

This data format is not used for MPEG-1, layer 3 audio, however (see MPEG-1 Layer 3 (MP3) Codecs in Sound sample data).

## MPEG-1 Sample Data

Each sample in an MPEG-1 media is an entire MPEG-1 stream. This means that a single MPEG-1 sample may be several hundred megabytes in size. The MPEG-1 encoding used by QuickTime corresponds to the ISO standard, as described in ISO document CD 11172.

## See Also

### Video and sound

Video media

Store compressed and uncompressed image data in QuickTime movies.

Sound media

Store compressed and uncompressed audio data in QuickTime movies.

Music media

Store note-based audio data, such as MIDI data, in QuickTime movies.

Movie media

Movie media is used to encapsulate embedded movies within QuickTime movies.

Defining media data layouts

Use efficient media layouts.

