

- AppKit
- NSTextTableBlock
-  init(table:startingRow:rowSpan:startingColumn:columnSpan:) 

Initializer

# init(table:startingRow:rowSpan:startingColumn:columnSpan:)

Returns an initialized text table block.

macOS

``` source
init(
    table: NSTextTable,
    startingRow row: Int,
    rowSpan: Int,
    startingColumn col: Int,
    columnSpan colSpan: Int
)
```

## Parameters 

`table`  

The text table containing this text table block.

`row`  

The table row at which the text table block starts.

`rowSpan`  

How many rows the text table block covers.

`col`  

The table column at which the text table block starts.

`colSpan`  

How many columns the text table block covers.

## Discussion

This is the designated initializer.

## See Also

### Related Documentation

Text Layout Programming Guide

