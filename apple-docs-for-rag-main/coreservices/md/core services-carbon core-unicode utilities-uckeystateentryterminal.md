

- Core Services
- Carbon Core
- Unicode Utilities
-  UCKeyStateEntryTerminal 

Structure

# UCKeyStateEntryTerminal

Maps from a dead-key state to the Unicode character(s) produced when that state is terminated by a given character key for a `'uchr'` resource.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct UCKeyStateEntryTerminal
```

## Overview

The `UCKeyStateEntryTerminal` type is used in the `stateEntryData[]` field of a structure of type UCKeyStateRecord. You should use the `UCKeyStateEntryTerminal` format for simple dead-key states that are terminated by a single keystroke, as in the U.S. keyboard layout. Each entry maps from the current dead-key state to the Unicode character(s) produced when a given character key is pressed that terminates the dead-key state.

## Topics

### Initializers

init()

init(curState: UInt16, charData: UCKeyCharSeq)

### Instance Properties

var charData: UCKeyCharSeq

A value of type `UCKeyCharSeq` specifying the Unicode character(s) produced when a given character key is pressed.

var curState: UInt16

An unsigned 16-bit integer specifying the current dead-key state.

