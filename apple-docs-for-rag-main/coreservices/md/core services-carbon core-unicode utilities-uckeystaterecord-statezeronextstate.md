

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeyStateRecord
-  stateZeroNextState 

Instance Property

# stateZeroNextState

An unsigned 16-bit integer specifying the dead-key state produced from a given key code when no previous dead-key state is in effect. If the `UCKeyStateRecord` structure does not initiate a dead-key state (but only provides terminators for other dead-key states), this will be 0. A non-zero value specifies the resulting new dead-key state and refers to the current state entry within the `stateEntryData[]` field for the following dead-key state record that is applied.

Mac Catalyst 13.0+macOS 10.0+

``` source
var stateZeroNextState: UInt16
```

