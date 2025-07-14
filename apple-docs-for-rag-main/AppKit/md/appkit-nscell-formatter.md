

- AppKit
- NSCell
-  formatter 

Instance Property

# formatter

The cell’s formatter object.

macOS

``` source
@MainActor
var formatter: Formatter? { get set }
```

## Discussion

A formatter handles the translation of the receiver’s contents between its onscreen representation and its object value. Cells use a formatter object to format the textual representation of their object value and to validate cell input and convert that input to an object value. When assigning a new formatter to a cell, the formatter attempts to interpret the cell’s current value. If it cannot do so, the formatter converts the current value to a string object.

