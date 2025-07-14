

- Core Services
- Carbon Core
- Unicode Utilities
-  Key Output Index Masks 

# Key Output Index Masks

Test the bits in `UCKeyOutput` values.

## Overview

You can use these masks to test the bits in `UCKeyOutput` values.

## Topics

### Constants

var kUCKeyOutputStateIndexMask: Int

If the bit specified by this mask is set, the UCKeyStateRecordsIndex `UCKeyOutput` value contains an index into a structure of type UCKeyStateRecordsIndex.

var kUCKeyOutputSequenceIndexMask: Int

If the bit specified by this mask is set, the `UCKeyOutput` value contains an index into a structure of type UCKeySequenceDataIndex.

var kUCKeyOutputTestForIndexMask: Int

var kUCKeyOutputGetIndexMask: Int

You can use this mask to test the bits (0–13) in a `UCKeyOutput` value that provide the actual index to another structure.

