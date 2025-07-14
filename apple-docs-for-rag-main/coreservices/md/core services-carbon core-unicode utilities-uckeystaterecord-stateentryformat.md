

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeyStateRecord
-  stateEntryFormat 

Instance Property

# stateEntryFormat

An unsigned 16-bit integer specifying the format of the data in the `stateEntryData` field’s array. This should be 0 if the `stateEntryCount` field is set to 0. Currently available values are `kUCKeyStateEntryTerminalFormat` and `kUCKeyStateEntryRangeFormat`; see Key State Entry Formats for descriptions of these values.

Mac Catalyst 13.0+macOS 10.0+

``` source
var stateEntryFormat: UInt16
```

