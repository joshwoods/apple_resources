

- QuickTime File Format
- Sample dependency flags atom ('sdtp')
-  Sample dependency flags table 

Data field

# Sample dependency flags table

A table of 8-bit values indicating the sample flag settings.

## Overview

The number of entries in the table is obtained from the associated sample size atom’s number of samples field.

An example of a sample dependency flags table is as follows.

| Sample dependency flag | Sample   |
|------------------------|----------|
| Flags                  | Sample 1 |
| Flags                  | Sample 2 |
| Flags                  | Sample 3 |
| Flags                  | Sample 4 |
| Flags                  | Sample 5 |

Flag values are specified as follows.

```
```

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the sample dependency flags atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this atom.

Flags

A 3-byte space reserved for flags.

