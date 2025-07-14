

- QuickTime File Format
-  Sample-to-chunk atom ('stsc') 

Atom

# Sample-to-chunk atom ('stsc')

An atom that stores chunk information for the samples in a media.

## Overview

As samples are added to a media, they are collected into chunks that allow optimized data access. A chunk contains one or more samples. Chunks in a media may have different sizes, and the samples within a chunk may have different sizes. The sample-to-chunk atom stores chunk information for the samples in a media.

Sample-to-chunk atoms have an atom type of `'stsc'`. The sample-to-chunk atom contains a table that maps samples to chunks in the media data stream. By examining the sample-to-chunk atom, you can determine the chunk that contains a specific sample.

The layout of the sample-to-chunk atom is as follows.

| Sample-to-chunk atom data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'stsc'` | 4 |
| Version | 1 |
| Flags | 3 |
| Number of entries | 4 |
| Sample-to-chunk table | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample-to-chunk atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample-to-chunk atom.

Flags

A 3-byte space for sample-to-chunk flags.

Number of entries

A 32-bit integer containing the count of entries in the sample-to-chunk table.

Sample-to-chunk table

A table that maps samples to chunks.

## See Also

### Describing samples

Sample table atom ('stbl')

An atom that contains information for converting from media time to sample number to sample location.

Seeking with a QuickTime file

Seek with a QuickTime file using child atoms.

Sample description atom ('stsd')

An atom that stores information that allows you to decode samples in the media.

Time-to-sample atom ('stts')

An atom that stores duration information for a media’s samples, providing a mapping from a time in a media to the corresponding data sample.

Creating video tracks at 30 frames per second

Configure your time-to-sample atom for 30 frames per second.

Creating video tracks at 29.97 frames per second

Configure your time-to-sample atom for 29.97 frames per second.

Creating sound tracks at 44.1 kHz

Configure your time-to-sample atom for sound at 44.1 kHz.

Composition offset atom ('ctts')

An atom you use to specify out-of-order video samples.

Composition shift least greatest atom ('cslg')

An atom that summarizes the calculated minimum and maximum offsets between decode and composition time, as well as the start and end times, for all samples.

Using composition offset and composition shift least greatest atoms

Calculate the offset shift when you store an out of order video stream’s sample table.

Sync sample atom ('stss')

An atom that identifies the key frames in the media.

Partial sync sample atom ('stps')

An atom that lists the partial sync samples.

Referencing two data files with a single track

Use multiple sample descriptions reference data in multiple files for a track.

Sample size atom ('stsz')

An atom you use to specify the size of each sample in the media.

Chunk offset atom ('stco')

An atom that identifies the location of each chunk of data in the media’s data stream.

