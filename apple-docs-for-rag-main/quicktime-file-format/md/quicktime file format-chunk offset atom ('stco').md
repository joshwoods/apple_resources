

- QuickTime File Format
-  Chunk offset atom ('stco') 

Atom

# Chunk offset atom ('stco')

An atom that identifies the location of each chunk of data in the media’s data stream.

## Overview

Chunk offset atoms have an atom type of `'stco'`.

The chunk-offset table gives the index of each chunk into the containing file. There are two variants, permitting the use of 32-bit or 64-bit offsets. The latter is useful when managing very large movies. Only one of these variants occurs in any single instance of a sample table atom.

Note that offsets are file offsets, not the offset into any atom within the file (for example, a `'mdat'` atom). This permits referring to media data in files without any atom structure. However, be careful when constructing a self-contained QuickTime file with its metadata (movie atom) at the front because the size of the movie atom affects the chunk offsets to the media data.

Note

The sample table atom can contain a 64-bit chunk offset atom (`STChunkOffset64AID = 'co64'`). When this atom appears, it is used in place of the original chunk offset atom, which can contain only 32-bit offsets. When QuickTime writes movie files, it uses the 64-bit chunk offset atom only if there are chunks that use the high 32-bits of the chunk offset. Otherwise, the original 32-bit chunk offset atom is used to ensure compatibility with previous versions of QuickTime.

The layout of a chunk offset atom is as follows.

| Chunk offset atom data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'stco'` | 4 |
| Version | 1 |
| Flags | 3 |
| Number of entries | 4 |
| Chunk offset table | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this chunk offset atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this chunk offset atom.

Flags

A 3-byte space for chunk offset flags.

Number of entries

A 32-bit integer containing the count of entries in the chunk offset table.

Chunk offset table

A chunk offset table consisting of an array of offset values.

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

Sample-to-chunk atom ('stsc')

An atom that stores chunk information for the samples in a media.

Referencing two data files with a single track

Use multiple sample descriptions reference data in multiple files for a track.

Sample size atom ('stsz')

An atom you use to specify the size of each sample in the media.

