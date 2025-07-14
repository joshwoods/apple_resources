

- Core Services
- Carbon Core
- Unicode Utilities
-  UCKeyStateRecordsIndex 

Structure

# UCKeyStateRecordsIndex

Provides a count of, and offsets to, dead-key state records in a `'uchr'` resource.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct UCKeyStateRecordsIndex
```

## Overview

The Unicode keyboard-layout (`'uchr'`) resource contains the data necessary to map virtual key codes to Unicode character codes for a given keyboard layout. The `'uchr'` format consists of a header information section and five key mapping data sections. The `UCKeyStateRecordsIndex` type is used in the third key mapping section of the `'uchr'` resource.

The `UCKeyStateRecordsIndex` structure is an index to dead-key state records of type UCKeyStateRecord. Any keycode-modifier combination which initiates a dead-key state or which is a valid terminator of a dead-key state refers to one of these records, via the `UCKeyStateRecordsIndex` structure.

## Topics

### Initializers

init()

init(keyStateRecordsIndexFormat: UInt16, keyStateRecordCount: UInt16, keyStateRecordOffsets: UInt32)

### Instance Properties

var keyStateRecordCount: UInt16

An unsigned 16-bit integer specifying the number of dead-key state records that are included in the resource.

var keyStateRecordOffsets: UInt32

An array of offsets from the beginning of the resource to each of the `UCKeyStateRecord` values that follow this structure in the `'uchr'` resource.

var keyStateRecordsIndexFormat: UInt16

An unsigned 16-bit integer identifying the format of the `UCKeyStateRecordsIndex` structure. Set to `kUCKeyStateRecordsIndexFormat`.

