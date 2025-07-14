

- AppKit
- NSGridView
-  cell(atColumnIndex:rowIndex:) 

Instance Method

# cell(atColumnIndex:rowIndex:)

Returns the grid cell object at the specified column and row index.

macOS 10.12+

``` source
@MainActor
func cell(
    atColumnIndex columnIndex: Int,
    rowIndex: Int
) -> NSGridCell
```

## See Also

### Creating and Merging Cells

func cell(for: NSView) -> NSGridCell?

Returns the grid cell object that contains the given view or one of its ancestors.

func mergeCells(inHorizontalRange: NSRange, verticalRange: NSRange)

Expands the cell at the top-leading corner of the horizontal and vertical range to cover the entire area.

