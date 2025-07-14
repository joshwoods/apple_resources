

- Core Services
- Carbon Core
- Unicode Utilities
-  UCKeyboardTypeHeader 

Structure

# UCKeyboardTypeHeader

Specifies a range of physical keyboard types in a `'uchr'` resource.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct UCKeyboardTypeHeader
```

## Overview

The `UCKeyboardTypeHeader` type is used in a structure of type UCKeyboardLayout to specify a range of physical keyboard types and contains offsets to each of the key mapping sections to be used for that range of keyboard types. Typically, you use an array of `UCKeyboardTypeHeader` structures, of which the first entry in the array is the default and will be used if the keyboard type does not fall within the range for any other entry. See UCKeyboardLayout for a further discussion of the context for use of the `UCKeyboardTypeHeader` type.

## Topics

### Initializers

init()

init(keyboardTypeFirst: UInt32, keyboardTypeLast: UInt32, keyModifiersToTableNumOffset: UInt32, keyToCharTableIndexOffset: UInt32, keyStateRecordsIndexOffset: UInt32, keyStateTerminatorsOffset: UInt32, keySequenceDataIndexOffset: UInt32)

### Instance Properties

var keyModifiersToTableNumOffset: UInt32

An unsigned 32-bit integer providing an offset to a structure of type UCKeyModifiersToTableNum. The `'uchr'` resource requires a `UCKeyModifiersToTableNum` structure, therefore this field must contain a non-zero value.

var keySequenceDataIndexOffset: UInt32

An unsigned 32-bit integer providing an offset to a structure of type UCKeySequenceDataIndex, if such is used in the resource. This value may be 0 if no character key sequences are included in the resource.

var keyStateRecordsIndexOffset: UInt32

An unsigned 32-bit integer providing an offset to a structure of type UCKeyStateRecordsIndex, if such is used in the resource. This value may be 0 if no dead-key state records are included in the resource.

var keyStateTerminatorsOffset: UInt32

An unsigned 32-bit integer providing an offset to a structure of type UCKeyStateTerminators, if such is used in the resource. This value may be 0 if no dead-key state terminators are included in the resource.

var keyToCharTableIndexOffset: UInt32

An unsigned 32-bit integer providing an offset to a structure of type UCKeyToCharTableIndex. The `'uchr'` resource requires a `UCKeyToCharTableIndex` structure, therefore this field must contain a non-zero value.

var keyboardTypeFirst: UInt32

An unsigned 32-bit integer specifying the first keyboard type in this entry. For the initial entry (that is, the default entry) in an array of `UCKeyboardTypeHeader` structures, you should set this value to 0. The initial `UCKeyboardTypeHeader` entry is used if the keyboard type passed to the function UCKeyTranslate(_:_:_:_:_:_:_:_:_:_:) does not match any other entry, that is, if it is not within the range of values specified by `keyboardTypeFirst` and `keyboardTypeLast` for any entry.

var keyboardTypeLast: UInt32

An unsigned 32-bit integer specifying the last keyboard type in this entry. For the initial entry (that is, the default entry) in an array of `UCKeyboardTypeHeader` structures, you should set this value to 0.

