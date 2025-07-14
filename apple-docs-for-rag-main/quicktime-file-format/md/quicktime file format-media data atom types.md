

- QuickTime File Format
-  Media data atom types 

API Collection

# Media data atom types

Store different types of media data, including video, sound, subtitles, and more.

## Overview

QuickTime uses atoms of different types to store different types of media data—video media atoms for video data, sound media atoms for audio data, and so on. Review the following topics to understand the fundamentals of how QuickTime uses atoms for storage of different types of media data.

## Topics

### Video and sound

Video media

Store compressed and uncompressed image data in QuickTime movies.

Sound media

Store compressed and uncompressed audio data in QuickTime movies.

Music media

Store note-based audio data, such as MIDI data, in QuickTime movies.

MPEG-1 media

Store MPEG-1 video streams, MPEG-1, layer 2 audio streams, and multiplexed MPEG-1 audio and video streams in QuickTime movies.

Movie media

Movie media is used to encapsulate embedded movies within QuickTime movies.

Defining media data layouts

Use efficient media layouts.

### Time-specific media

Timed metadata media

Store timed metadata in QuickTime movies with a track structure.

Timecode media

Store time code data in QuickTime movies with timecode media.

### Text, captions, and subtitles

Text media

Store text data in QuickTime movies.

Closed captioning media

Store closed captioning for QuickTime movies.

Subtitle media

Store text data used for subtitles in QuickTime movies.

### Track features

Modifier tracks

Create dynamic movies with modifier tracks that send data to another track.

Creating movies with modifier tracks

Send data to another media handler instead of presenting media directly.

Track references

Relate a movie’s tracks to one another with track references.

Chapter lists

A chapter list provides a set of named entry points into a movie.

Streaming media

Store streaming data in a streaming media track for QuickTime movies.

### Hint media

Hint media

Provide information about data units to stream in hint tracks.

Finding an original media track from a hint track

Use track reference atoms from hint tracks to locate the original media track.

RTP hint tracks

Allow a streaming server to create RTP streams from a QuickTime movie.

Hint track sample description

An atom that specifies the data format and location of the hint track sample data.

Packetization hint sample data

An atom that describes the sample data for data using the Real-Time Transport Protocol (RTP).

