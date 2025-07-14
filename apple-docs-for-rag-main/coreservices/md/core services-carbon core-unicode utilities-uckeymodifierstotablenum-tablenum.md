

- Core Services
- Carbon Core
- Unicode Utilities
- UCKeyModifiersToTableNum
-  tableNum 

Instance Property

# tableNum

An array of unsigned 8-bit integers that map modifier bit combinations to table numbers. These values are indexes into the `keyToCharTableOffsets` array in a UCKeyToCharTableIndexstructure; these, in turn, are offsets to the actual key-code-to character tables, which follow the `UCKeyToCharTableIndex` structure in the `'uchr'` resource.

Mac Catalyst 13.0+macOS 10.0+

``` source
var tableNum: UInt8
```

