

- QuickTime File Format
-  Sample table atom ('stbl') 

Atom

# Sample table atom ('stbl')

An atom that contains information for converting from media time to sample number to sample location.

## Mentioned in 

Tween sample description

3D media

Streaming media

## Overview

This atom also indicates how to interpret the sample (for example, whether to decompress the video data and, if so, how). This section describes the format and content of the sample table atom.

The sample table atom has an atom type of `'stbl'`. It can contain the sample description atom, the time-to-sample atom, the sync sample atom, the sample-to-chunk atom, the sample size atom, the chunk offset atom, and the shadow sync atom. Recent additions to the list of atom types that a sample table atom can contain are the optional sample group description and sample-to-group atoms included in Audio priming-handling encoder delay in AAC.

The sample table atom contains all the time and data indexing of the media samples in a track. Using tables, it is possible to locate samples in time, determine their type, and determine their size, container, and offset into that container.

If the track that contains the sample table atom references no data, then the sample table atom does not need to contain any child atoms (not a very useful media track).

If the track that the sample table atom is contained in does reference data, then the following child atoms are required: sample description, sample size, sample to chunk, and chunk offset. All of the subtables of the sample table use the same total sample count.

The sample description atom must contain at least one entry. A sample description atom is required because it contains the data reference index field that indicates which data reference atom to use to retrieve the media samples. Without the sample description, it is not possible to determine where the media samples are stored. The sync sample atom is optional. If the sync sample atom is not present, all samples are implicitly sync samples.

The layout of the sample table atom is as follows.

| Data | Type |
|----|----|
| Size | 4 bytes |
| Type = `'stbl'` | 4 bytes |
| Sample description atom | `'stsd'` |
| Time-to-sample atom | `'stts'` |
| Composition offset atom | `'ctts'` |
| Composition shift least greatest atom | `'cslg'` |
| Sync sample atom | `'stss'` |
| Partial sync sample atom | `'stps'` |
| Sample-to-chunk atom | `'stsc'` |
| Sample size atom | `'stsz'` |
| Chunk offset atom | `'stco'` |
| Sample dependency flags atom | `'sdtp'` |
| Shadow sync atom | `'stsh'` |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample table atom.

Type

A 32-bit integer that identifies the atom type.

Sample description atom

An atom that stores information that allows you to decode samples in the media.

Time-to-sample atom

An atom that stores duration information for a media’s samples, providing a mapping from a time in a media to the corresponding data sample.

Composition offset atom

An atom you use to specify out-of-order video samples.

Composition shift least greatest atom

An atom that summarizes the calculated minimum and maximum offsets between decode and composition time, as well as the start and end times, for all samples.

Sync sample atom

An atom that identifies the key frames in the media.

Partial sync sample atom

An atom that lists the partial sync samples.

Sample-to-chunk atom

An atom that stores chunk information for the samples in a media.

Sample size atom

An atom you use to specify the size of each sample in the media.

Chunk offset atom

An atom that identifies the location of each chunk of data in the media’s data stream.

Sample dependency flags atom

An atom that uses one byte per sample as a bit field that describes dependency information.

Shadow sync atom

An atom reserved for future use.

## See Also

### Describing samples

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

Sample-to-chunk atom ('stsc')

An atom that stores chunk information for the samples in a media.

Referencing two data files with a single track

Use multiple sample descriptions reference data in multiple files for a track.

Sample size atom ('stsz')

An atom you use to specify the size of each sample in the media.

Chunk offset atom ('stco')

An atom that identifies the location of each chunk of data in the media’s data stream.

