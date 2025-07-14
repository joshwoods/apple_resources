

- AppKit
- NSTableView
- NSTableView.ColumnAutoresizingStyle
-  NSTableView.ColumnAutoresizingStyle.lastColumnOnlyAutoresizingStyle 

Case

# NSTableView.ColumnAutoresizingStyle.lastColumnOnlyAutoresizingStyle

Autoresize only the last table column.

macOS

``` source
case lastColumnOnlyAutoresizingStyle
```

## Discussion

When that table column can no longer be resized, stop autoresizing. Normally you should use one of the sequential autoresizing modes instead.

## See Also

### Constants

case noColumnAutoresizing

Disable table column autoresizing.

case uniformColumnAutoresizingStyle

Autoresize all columns by distributing space equally, simultaneously.

case sequentialColumnAutoresizingStyle

Autoresize each table column sequentially, from the last auto-resizable column to the first auto-resizable column; proceed to the next column when the current column has reached its minimum or maximum size.

case reverseSequentialColumnAutoresizingStyle

Autoresize each table column sequentially, from the first auto-resizable column to the last auto-resizable column; proceed to the next column when the current column has reached its minimum or maximum size.

case firstColumnOnlyAutoresizingStyle

Autoresize only the first table column.

