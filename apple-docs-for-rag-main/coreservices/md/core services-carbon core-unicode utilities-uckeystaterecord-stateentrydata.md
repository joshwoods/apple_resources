

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeyStateRecord
-  stateEntryData 

Instance Property

# stateEntryData

An array of dead-key state entries, whose size depends on their format, but which will always be a multiple of 4 bytes. Each entry maps from the current dead-key state to the Unicode character(s) that result when a given character key is pressed or to the next dead-key state, if any. The format of the entry is specified by the `stateEntryFormat` field to be either that of type UCKeyStateEntryTerminal or UCKeyStateEntryRange.

Mac Catalyst 13.0+macOS 10.0+

``` source
var stateEntryData: UInt32
```

