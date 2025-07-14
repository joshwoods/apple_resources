

- QuickTime File Format
- Partial sync sample atom ('stps')
-  Partial sync sample table 

Data field

# Partial sync sample table

A table of sample numbers.

## Overview

The layout of a partial sync sample table is as follows.

| Sample number | Sample   |
|---------------|----------|
| Number        | Sample 1 |
| Number        | Sample 2 |
| Number        | Sample 3 |
| Number        | Sample 4 |
| Number        | Sample 5 |

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the partial sync sample atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this atom.

Flags

A 3-byte space reserved for flags.

Entry count

A 32-bit unsigned integer that specifies the number of sample numbers in the array that follows.

