

- QuickTime File Format
- Edit list atom ('elst')
-  Edit list table 

Data field

# Edit list table

An array of 32-bit values, grouped into entries containing 3 values each.

## Mentioned in 

Representing encoder delay explicitly

## Overview

The layout of the entries in this table is as follows.

| Field          | Bytes |
|----------------|-------|
| Track duration | 4     |
| Media time     | 4     |
| Media rate     | 4     |

An edit list table entry contains the following elements.

Track duration  
A 32-bit integer that specifies the duration of this edit segment in units of the movie’s time scale.

Media time  
A 32-bit integer containing the starting time within the media of this edit segment (in media timescale units). If this field is set to `–1`, it is an empty edit. The last edit in a track should never be an empty edit. Any difference between the movie’s duration and the track’s duration is expressed as an implicit empty edit.

Media rate  
A 32-bit fixed-point number that specifies the relative rate at which to play the media corresponding to this edit segment. This rate value cannot be `0` or negative.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this edit list atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this edit list atom.

Flags

Three bytes of space for flags.

Number of entries

A 32-bit integer that specifies the number of entries in the edit list atom.

