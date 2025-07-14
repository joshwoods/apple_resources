

- AppKit
- NSTableView
- NSTableView.ColumnAutoresizingStyle
-  NSTableView.ColumnAutoresizingStyle.sequentialColumnAutoresizingStyle 

Case

# NSTableView.ColumnAutoresizingStyle.sequentialColumnAutoresizingStyle

Autoresize each table column sequentially, from the last auto-resizable column to the first auto-resizable column; proceed to the next column when the current column has reached its minimum or maximum size.

macOS

``` source
case sequentialColumnAutoresizingStyle
```

## See Also

### Constants

case noColumnAutoresizing

Disable table column autoresizing.

case uniformColumnAutoresizingStyle

Autoresize all columns by distributing space equally, simultaneously.

case reverseSequentialColumnAutoresizingStyle

Autoresize each table column sequentially, from the first auto-resizable column to the last auto-resizable column; proceed to the next column when the current column has reached its minimum or maximum size.

case lastColumnOnlyAutoresizingStyle

Autoresize only the last table column.

case firstColumnOnlyAutoresizingStyle

Autoresize only the first table column.

