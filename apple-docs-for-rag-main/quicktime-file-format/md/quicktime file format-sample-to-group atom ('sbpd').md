

- QuickTime File Format
-  Sample-to-group atom ('sbpd') 

Atom

# Sample-to-group atom ('sbpd')

An atom that associates a sample with a sample group description.

## Mentioned in 

Representing encoder delay explicitly

## Overview

Sample-to-group atoms are used to find the group that a sample belongs to and the associated description of that sample group. The sample-to-group atom has an atom type of `‘sbgp’`.

In a general case, there may be multiple instances of sample-to-group atoms if there is more than one sample grouping for the samples in a track. Each instance of the sample-to group atom has a grouping type code that distinguishes different sample groupings. Within a track there can be at most one instance of this atom with a particular grouping type. An associated sample group description atom indicates the same value for the grouping type.

The sample-to-group atom contains a table with a sample count and group description index pairs. The sample count is the number of media samples in the run of samples with the same sample group description. The group description index is an index into the array of payload data entries in the associated sample group description atom’s payload data table, the association defined by having the same grouping type value.

For use in AAC encoder delay representation, there is one sample-to-group atom instance in a given QuickTime sound track with grouping type `‘roll’` matching the single instance of the sample group description atom. The entry count field value is set to `1`, indicating one entry in the table data array. That entry is describing all the AAC packets in the track. The sample count in the table data array is typically the same as the sample size atom’s number of entries field, see Sample size atom ('stsz'), which represents the number of media samples in the track (in this use, AAC packets). For AAC encoder delay representation, the only entry in the associated sample group description atom’s payload data table is the first, which provides the value of 1 for the group description index.

The layout of the sample-to-group atom is as follows:

| Sample-to-group atom | Bytes |
|----|----|
| Size | 4 |
| Type = `'sbgp'` | 4 |
| Version | 1 |
| Flags | 3 |
| Grouping type | 4 |
| Default length | 4 |
| Entry count | 4 |
| Table data | variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample-to-group atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample-to-group atom.

Flags

A 3-byte reserved space.

Grouping type

A 32-bit integer identifying the grouping type.

Default length

A 32-bit integer indicating the length of the group entry in the payload data.

Entry count

A 32-bit integer giving the number of entries in the table data that follows.

Table data

A table of sample count and group description index pairs.

## See Also

### Sample group structures

Sample group description atom ('sgpd')

An atom that gives information about the characteristics of sample groups.

