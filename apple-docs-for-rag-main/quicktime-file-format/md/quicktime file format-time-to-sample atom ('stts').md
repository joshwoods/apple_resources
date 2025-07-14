

- QuickTime File Format
-  Time-to-sample atom ('stts') 

Atom

# Time-to-sample atom ('stts')

An atom that stores duration information for a media’s samples, providing a mapping from a time in a media to the corresponding data sample.

## Overview

Time-to-sample atoms store duration information for a media’s samples, providing a mapping from a time in a media to the corresponding data sample. The time-to-sample atom has an atom type of `'stts'`.

You can determine the appropriate sample for any time in a media by examining the time-to-sample atom table, which is contained in the time-to-sample atom.

The atom contains a compact version of a table that allows indexing from time to sample number. Other tables provide sample sizes and pointers from the sample number. Each entry in the table gives the number of consecutive samples with the same time delta, and the delta of those samples. By adding the deltas, a complete time-to-sample map can be built.

The atom contains time deltas: `DT(n+1) = DT(n) + STTS(n)` where `STTS(n)` is the (uncompressed) table entry for sample `n` and `DT` is the display time for sample `(n)`. The sample entries are ordered by time stamps; therefore, the deltas are all nonnegative. The `DT` axis has a zero origin; `DT(i) = SUM` (for `j=0` to `i-1` of `delta(j)`), and the sum of all deltas gives the length of the media in the track (not mapped to the overall time scale, and not considering any edit list). The edit list atom provides the initial DT value if it is nonempty (nonzero).

The layout of the time-to-sample atom is as follows.

| Time-to-sample atom data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'ctts'` | 4 |
| Version | 1 |
| Flags | 3 |
| Number of entries | 4 |
| Time-to-sample table | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this time-to-sample atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this time-to-sample atom.

Flags

A 3-byte space for time-to-sample flags.

Number of entries

A 32-bit integer containing the count of entries in the time-to-sample table.

Time-to-sample table

A table that defines the duration of each sample in the media.

## See Also

### Describing samples

Sample table atom ('stbl')

An atom that contains information for converting from media time to sample number to sample location.

Seeking with a QuickTime file

Seek with a QuickTime file using child atoms.

Sample description atom ('stsd')

An atom that stores information that allows you to decode samples in the media.

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

Sample-to-chunk atom ('stsc')

An atom that stores chunk information for the samples in a media.

Referencing two data files with a single track

Use multiple sample descriptions reference data in multiple files for a track.

Sample size atom ('stsz')

An atom you use to specify the size of each sample in the media.

Chunk offset atom ('stco')

An atom that identifies the location of each chunk of data in the media’s data stream.

