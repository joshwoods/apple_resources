

- QuickTime File Format
- Sample table atom ('stbl')
-  Sync sample atom 

Data field

# Sync sample atom

An atom that identifies the key frames in the media.

## Overview

See Sync sample atom ('stss').

## See Also

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

