

- QuickTime File Format
- Sample atoms
-  Creating sound tracks at 44.1 kHz 

Article

# Creating sound tracks at 44.1 kHz

Configure your time-to-sample atom for sound at 44.1 kHz.

## Overview

The duration of an audio sample is stored in the time-to-sample atom contained in a sample table atom. This duration cannot be interpreted without the media’s time scale, which defines the units per second for the duration. With audio, the duration of each audio sample is typically `1`, so the time-to-sample atom has one entry, which applies to all audio samples.

With a time scale of `44100` in the media header atom, the time-to-sample atom would contain the data values listed in the following table.

| Field             | Value    |
|-------------------|----------|
| Atom size         | `24`     |
| Atom type         | `'stts'` |
| Version/Flags     | `0`      |
| Number of entries | `1`      |
| Sample count      | `n`      |
| Sample duration   | `1`      |

This atom does not indicate whether the audio is stereo or mono or whether it contains 8-bit or 16-bit samples. That information is stored in the sound sample description atom, which is contained in the sample table atom.

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

