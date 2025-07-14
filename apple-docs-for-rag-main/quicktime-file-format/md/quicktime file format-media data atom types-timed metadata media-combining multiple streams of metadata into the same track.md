

- QuickTime File Format
- Media data atom types
- Timed metadata media
-  Combining multiple streams of metadata into the same track 

Article

# Combining multiple streams of metadata into the same track

Introduce new metadata samples with the union of all metadata values from combined tracks.

## Overview

Because two “streams” or tracks of metadata values might occur where the time ranges for one stream does not coincide with those of the other stream, a convention is recommended if both streams of metadata values are combined into a single new metadata track (typically because of some production process). At any point in the timeline where a metadata value comes into scope or goes out of scope, new metadata samples should be introduced with the union of all metadata values present for the time range, replacing the existing overlapped samples for that portion of the media time range.

For example, this figure shows the results of combining the metadata from two metadata tracks:

Note

The combined timed metadata media samples from time t1 to t2 contain both the A and B metadata values. This is done so that for any time t, it is possible to determine all applicable metadata values without needing to scan through all timed metadata media tracks in backward or forward directions.

In the new combined track, a single timed metadata sample description containing the keys A and B may be used. Creating sample descriptions for each combination (A, B, {A,B}) is possible but discouraged as this makes the determination of whether a key is in the tracks more complex.

## See Also

### Storing timed metadata media

Overview of timed metadata

Synchronize metadata references to media tracks for particular media time periods with timed metadata.

Timed metadata sample description

An atom that defines how to interpret timed metadata media samples.

Timed metadata sample data format

A concatenation of one or more atoms that structure a timed metadata media sample.

Constant-size timed metadata sample data

Create metadata tracks with samples that have the same size.

Movie-level relationships among tracks

Handling tracks with more than one associated metadata track.

