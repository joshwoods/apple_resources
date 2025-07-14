

- AppKit
- NSGridView
-  cell(for:) 

Instance Method

# cell(for:)

Returns the grid cell object that contains the given view or one of its ancestors.

macOS 10.12+

``` source
@MainActor
func cell(for view: NSView) -> NSGridCell?
```

## See Also

### Creating and Merging Cells

func cell(atColumnIndex: Int, rowIndex: Int) -> NSGridCell

Returns the grid cell object at the specified column and row index.

func mergeCells(inHorizontalRange: NSRange, verticalRange: NSRange)

Expands the cell at the top-leading corner of the horizontal and vertical range to cover the entire area.

