

- QuickTime File Format
-  Composition shift least greatest atom ('cslg') 

Atom

# Composition shift least greatest atom ('cslg')

An atom that summarizes the calculated minimum and maximum offsets between decode and composition time, as well as the start and end times, for all samples.

## Overview

The optional composition shift least greatest atom summarizes the calculated minimum and maximum offsets between decode and composition time, as well as the start and end times, for all samples. This allows a reader to determine the minimum required time for decode to obtain proper presentation order without needing to scan the sample table for the range of offsets. The type of the composition shift least greatest atom is `‘cslg’`.

The layout of a composition shift least greatest atom is as follows.

| Composition shift least greatest atom data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'cslg'` | 4 |
| Version | 1 |
| Flags | 3 |
| compositionOffsetToDisplayOffsetShift | 4 |
| leastDisplayOffset | 4 |
| greatestDisplayOffset | 4 |
| displayStartTime | 4 |
| displayEndTime | 4 |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the composition shift least greatest atom atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this atom.

Flags

A 3-byte space reserved for flags.

compositionOffsetToDisplayOffsetShift

A 32-bit unsigned integer that specifies the calculated value.

leastDisplayOffset

A 32-bit unsigned integer that specifies the calculated value.

greatestDisplayOffset

A 32-bit unsigned integer that specifies the calculated value.

displayStartTime

A 32-bit signed integer that specifies the calculated value.

displayEndTime

A 32-bit signed integer that specifies the calculated value.

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

