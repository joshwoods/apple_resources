

- QuickTime File Format
- Metadata atoms and types
- Metadata handling
-  Digital video file formats 

Article

# Digital video file formats

## Overview

| OpenDML and other AVI files | Description |
|----|----|
|  |  |
| Supported by | Movie import component |
| Macintosh file type | `'VfW '` |
| File name extensions | .avi |
| metadata handling | All Microsoft-defined “tombstone” data is transferred to the imported movie’s user data. Metadata fields that have QuickTime equivalents are mapped as follows: `'ICOP'` maps to `kUserDataTextCopyright`, `'ISBJ'` maps to `kUserDataTextInformation`, `'INAM'` maps to `kUserDataTextFullName`, `'ICRD'` maps to `'©day'`, `'IMED'` maps to `'©fmt'`, `'ISRC'` maps to `'©src'`. Where no QuickTime equivalent exists, the metadata item’s four-character code is modified by replacing the initial `I` with the symbol `©`. All other characters remain unchanged. |
| Software required | QuickTime 3 |

## See Also

### Handling metadata

Digital audio file formats

Still image file formats

Animation and 3D file formats

