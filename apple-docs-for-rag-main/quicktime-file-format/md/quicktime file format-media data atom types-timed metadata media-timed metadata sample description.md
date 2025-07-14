

- QuickTime File Format
- Media data atom types
- Timed metadata media
-  Timed metadata sample description 

API Collection

# Timed metadata sample description

An atom that defines how to interpret timed metadata media samples.

## Overview

The timed metadata sample description contains information that defines how to interpret timed metadata media samples. This sample description is based on the standard sample description header, as described in Sample description atom ('stsd').

The metadata sample description is a derived sample description format which describes metadata values represented in atoms. It may also include other atoms not holding metadata values.

Zero, one, or more values may be carried in a metadata sample description for a particular time.

The data format field contains the format of the timed metadata media, which is set to `'mebx'`.

Note

Other forms of timed metadata media are not described here. They would be indicated by an alternative type code in the place of `‘mebx’`.

The metadata sample description must contain a metadata key table atom and optionally contains a bit rate atom following the standard sample description atom header, defined below. Other atoms may be introduced in the future.

Metadata key table  
An atom containing a table of keys and mappings to payload data in the corresponding timed metadata media samples.

Bit rate atom  
An optional atom that contains data that signals the bit rate of a media stream.

## Topics

### Describing timed metadata

Metadata key table atom ('keys')

An atom that contains a table of keys and mappings to payload data in the corresponding timed metadata media samples.

Bit rate atom ('btrt')

An atom that signals the bit rate information of a stream.

Metadata key atom

An atom that contains a key that corresponds to the timed metadata track containing it.

Metadata key declaration atom ('keyd')

An atom that holds the key namespace and key value of that namespace for the given values.

Metadata datatype definition atom ('dtyp')

An atom you use to specify the data type of the metadata key atom’s value.

Metadata locale atom ('loca')

An atom that tags a metadata value with a locale.

## See Also

### Storing timed metadata media

Overview of timed metadata

Synchronize metadata references to media tracks for particular media time periods with timed metadata.

Timed metadata sample data format

A concatenation of one or more atoms that structure a timed metadata media sample.

Constant-size timed metadata sample data

Create metadata tracks with samples that have the same size.

Combining multiple streams of metadata into the same track

Introduce new metadata samples with the union of all metadata values from combined tracks.

Movie-level relationships among tracks

Handling tracks with more than one associated metadata track.

