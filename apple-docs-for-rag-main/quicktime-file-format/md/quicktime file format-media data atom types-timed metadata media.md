

- QuickTime File Format
- Media data atom types
-  Timed metadata media 

# Timed metadata media

Store timed metadata in QuickTime movies with a track structure.

## Overview

A track structure is used to store timed metadata in QuickTime movies. This section provides an overview of the timed metadata track structure, and describes the timed metadata sample descriptions and the storage format of timed metadata media samples. The timed metadata track structure has a media type of `‘meta’`.

## Topics

### Storing timed metadata media

Overview of timed metadata

Synchronize metadata references to media tracks for particular media time periods with timed metadata.

Timed metadata sample description

An atom that defines how to interpret timed metadata media samples.

Timed metadata sample data format

A concatenation of one or more atoms that structure a timed metadata media sample.

Constant-size timed metadata sample data

Create metadata tracks with samples that have the same size.

Combining multiple streams of metadata into the same track

Introduce new metadata samples with the union of all metadata values from combined tracks.

Movie-level relationships among tracks

Handling tracks with more than one associated metadata track.

## See Also

### Time-specific media

Timecode media

Store time code data in QuickTime movies with timecode media.

