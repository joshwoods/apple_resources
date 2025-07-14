

- AppKit
- NSTableView
- NSTableView.ColumnAutoresizingStyle
-  NSTableView.ColumnAutoresizingStyle.uniformColumnAutoresizingStyle 

Case

# NSTableView.ColumnAutoresizingStyle.uniformColumnAutoresizingStyle

Autoresize all columns by distributing space equally, simultaneously.

macOS

``` source
case uniformColumnAutoresizingStyle
```

## See Also

### Constants

case noColumnAutoresizing

Disable table column autoresizing.

case sequentialColumnAutoresizingStyle

Autoresize each table column sequentially, from the last auto-resizable column to the first auto-resizable column; proceed to the next column when the current column has reached its minimum or maximum size.

case reverseSequentialColumnAutoresizingStyle

Autoresize each table column sequentially, from the first auto-resizable column to the last auto-resizable column; proceed to the next column when the current column has reached its minimum or maximum size.

case lastColumnOnlyAutoresizingStyle

Autoresize only the last table column.

case firstColumnOnlyAutoresizingStyle

Autoresize only the first table column.

