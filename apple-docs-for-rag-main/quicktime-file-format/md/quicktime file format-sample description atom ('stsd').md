

- QuickTime File Format
-  Sample description atom ('stsd') 

Atom

# Sample description atom ('stsd')

An atom that stores information that allows you to decode samples in the media.

## Mentioned in 

Music media

Sprite media

QuickTime File Format change log

MPEG-1 media

## Overview

The data stored in the sample description varies, depending on the media type. For example, in the case of video media, the sample descriptions are image description structures. The sample description information for each media type is explained in Media data atom types.

The layout of the sample description atom is as follows.

| Sample description atom data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'stsd'` | 4 |
| Version | 1 |
| Flags | 3 |
| Number of entries | 4 |
| Sample description table | Variable |

The sample description atom has an atom type of `'stsd'`. The sample description atom contains a table of sample descriptions. A media may have one or more sample descriptions, depending upon the number of different encoding schemes used in the media and on the number of files used to store the data. The sample-to-chunk atom identifies the sample description for each sample in the media by specifying the index into this table for the appropriate description (see Sample-to-chunk atom ('stsc')).

## General structure of a sample description

While the exact format of the sample description varies by media type, the first four fields of every sample description are the same.

Sample description size  
A 32-bit integer indicating the number of bytes in the sample description.

Important

When parsing sample descriptions in the `‘stsd’` atom, be aware of the sample description size value in order to read each table entry correctly. Some sample descriptions terminate with four zero bytes that are not otherwise indicated.

Data format  
A 32-bit integer indicating the format of the stored data. This depends on the media type, but is usually either the compression format or the media type.

Reserved  
Six bytes that must be set to `0`.

Data reference index  
A 16-bit integer that contains the index of the data reference to use to retrieve data associated with samples that use this sample description. Data references are stored in data reference atoms.

These four fields may be followed by additional data specific to the media type and data format. See Media data atom types for additional details regarding specific media types and media formats.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample description atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample description atom.

Flags

A 3-byte space for sample description flags.

Number of entries

A 32-bit integer containing the number of sample descriptions that follow.

Sample description table

An array of sample descriptions.

## See Also

### Describing samples

Sample table atom ('stbl')

An atom that contains information for converting from media time to sample number to sample location.

Seeking with a QuickTime file

Seek with a QuickTime file using child atoms.

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

