

- QuickTime File Format
- Closed captioning sample data ('cdat')
-  Type 

Data field

# Type

A 32-bit integer that identifies the atom type.

## Overview

This field must be set to `'cdat'`.

Note

Apple reserves all atom types with lowercase letters and numbers.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this closed captioning media data atom.

Sample data

An array of one or more byte pairs for data channel 1/field 1 (“CC1”) of a CEA-608 data stream, each byte pair corresponding to a video frame.

