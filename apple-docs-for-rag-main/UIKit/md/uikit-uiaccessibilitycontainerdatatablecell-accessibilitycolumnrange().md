

- UIKit
- UIAccessibilityContainerDataTableCell
-  accessibilityColumnRange() 

Instance Method

# accessibilityColumnRange()

Returns the columns spanned by the cell.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func accessibilityColumnRange() -> NSRange
```

**Required**

## Return Value

The column or columns that the cell spans.

## Discussion

Set the location of the range to the first column containing the cell. Use the length of the range to specify the number of columns that the cell spans. If you do not implement this method, the system assumes an initial index of NSNotFound and a length of `0`.

## See Also

### Getting the rows and columns

func accessibilityRowRange() -> NSRange

Returns the visible range of rows.

**Required**

