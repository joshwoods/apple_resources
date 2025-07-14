

- QuickTime File Format
-  Composition offset atom ('ctts') 

Atom

# Composition offset atom ('ctts')

An atom you use to specify out-of-order video samples.

## Overview

Video samples in encoded formats have a decode order and a presentation order (also called composition order or display order). The composition offset atom is used when there are out-of-order video samples.

- If the decode and presentation orders are the same, no composition offset atom will be present. The time-to-sample atom provides both the decode and presentation ordering of the video stream, and allows calculation of the start and end times.

- If video samples are stored out of presentation order, the time-to-sample atom provides the decode order and the composition offset atom provides the time of presentation for the decoded samples expressed as a delta on a sample-by-sample basis.

Note

Decode time does not directly imply presentation time when working with out of order video samples. The ordering is significant.

The composition offset atom contains a sample-by-sample mapping of the decode-to-presentation time. Each entry in the composition offset table is a time delta from decode to presentation time: `CT(n) = DT(n) + CTTS(n)` where `CTTS(n)` is the (uncompressed) table entry for sample `n` `DT` is the decode time and `CT` is the composition (or display) time. The delta expressed in the composition offset table can be positive or negative.

When the time-to-sample atom and the composition offset atom are present, a reader parsing out-of-order video samples has all the information necessary to calculate the start and end times, as well as the minimum and maximum offsets between decode time and presentation time. The sample tables are scanned to obtain these values.

Note

At the last displayed frame, the decode duration is used as presentation duration.

The type of the composition offset atom is `‘ctts’`.

The layout of a composition offset atom is as follows.

| Composition offset atom data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'ctts'` | 4 |
| Version | 1 |
| Flags | 3 |
| Entry count | 4 |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the composition offset atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this atom.

Flags

A 3-byte space reserved for offset flags.

Entry count

A 32-bit unsigned integer that specifies the number of sample numbers in the array that follows.

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

