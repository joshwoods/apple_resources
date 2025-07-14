

- AppKit
- NSTableRowView
-  view(atColumn:) 

Instance Method

# view(atColumn:)

Provides access to the given view at a particular column.

macOS 10.7+

``` source
@MainActor
func view(atColumn column: Int) -> Any?
```

## Parameters 

`column`  

The index of the column.

## Return Value

The view for the specified column.

## Discussion

This is the only way to access cell views after the row view has been removed from the table.

