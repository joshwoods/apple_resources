

- QuickTime File Format
- Profile atom ('prfl')
-  Feature entries 

Data field

# Feature entries

A list of feature entries.

## Overview

Each feature entry consists of:

`reserved`  
A 32-bit field that must be set to zero.

`part-ID`  
Either a brand identifier that occurs in the file-type atom of the same file, indicating a feature that is specific to this brand, or the value `0x20202020` (four ASCII spaces) indicating a universal feature that can be found in any file type that allows the profile atom. The value 0 is reserved for an empty slot.

`feature-code`  
A four-character code either documented here (universal features), or in the specification identified by the brand. The value of `0` is reserved for an empty slot with no meaningful feature-value.

`feature-value`  
Either a value from an enumerated set (for example, `1` or `0` for `true` or `false`, or an MPEG-4 profile-level ID) or a value that can compared (for example, bit rate as an integer or dimensions as a 32-bit packed structure).

The following table shows the layout of a typical feature.

| Data field                   | Bytes |
|------------------------------|-------|
| Reserved = `0x00000000`      | 4     |
| Part ID = ’ ’ (`0x20202020`) | 4     |
| Feature code = `'avbr'`      | 4     |
| Value = `0x00000001`         | 4     |

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this atom.

Type

A 32-bit integer that identifies the atom type.

Version

An 8-bit integer that holds the version.

Flags

An 8-bit integer with flags.

Number of feature entries

A 32-bit integer that indicates how many feature entries are in the atom.

