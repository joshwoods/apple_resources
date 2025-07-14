

- AppKit
- NSGridView
-  mergeCells(inHorizontalRange:verticalRange:) 

Instance Method

# mergeCells(inHorizontalRange:verticalRange:)

Expands the cell at the top-leading corner of the horizontal and vertical range to cover the entire area.

macOS 10.12+

``` source
@MainActor
func mergeCells(
    inHorizontalRange hRange: NSRange,
    verticalRange vRange: NSRange
)
```

## Discussion

This function invalidates other cells in the range, and they no longer maintain their layout, constraints, or content views. Cell merging has no effect on the base cell coordinate system of the grid view, and cell references within a merged region refer to the single merged cell.

Use this method to configure the grid geometry before installing views. If the cells being merged contain content views, only the top-leading views are kept.

## See Also

### Creating and Merging Cells

func cell(atColumnIndex: Int, rowIndex: Int) -> NSGridCell

Returns the grid cell object at the specified column and row index.

func cell(for: NSView) -> NSGridCell?

Returns the grid cell object that contains the given view or one of its ancestors.

