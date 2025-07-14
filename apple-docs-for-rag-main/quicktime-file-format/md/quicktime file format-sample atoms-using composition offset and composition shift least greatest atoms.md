

- QuickTime File Format
- Sample atoms
-  Using composition offset and composition shift least greatest atoms 

Article

# Using composition offset and composition shift least greatest atoms

Calculate the offset shift when you store an out of order video stream’s sample table.

## Overview

Calculate the offset shift with code similar to the following example:

```
leastDisplayOffset = min { display offsets of all samples }
greatestDisplayOffset = max { display offsets of all samples }
if( leastDisplayOffset 

These values are stored in a composition shift least greatest atom within the sample table atom.

Then write a composition offset table atom that stores the display offsets, adjusting each offset by subtracting compositionOffsetToDisplayOffsetShift:

```
compositionOffset[n] = displayOffset[n] - compositionOffsetToDisplayOffsetShift;
```

Note

If a composition shift least greatest atom is not present, assume `compositionOffsetToDisplayOffsetShift = 0`. The sample tables will need to be scanned to find the least and greatest offsets, as well as the presentation start and end times, to determine the decode time offset required for presentation.

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

