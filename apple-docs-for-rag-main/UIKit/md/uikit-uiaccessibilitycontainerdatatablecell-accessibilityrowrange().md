

- UIKit
- UIAccessibilityContainerDataTableCell
-  accessibilityRowRange() 

Instance Method

# accessibilityRowRange()

Returns the visible range of rows.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func accessibilityRowRange() -> NSRange
```

**Required**

## Return Value

The visible range of rows.

## Discussion

Set the location of the range to the first row containing the cell. Use the length of the range to specify the number of rows that the cell spans. If you do not implement this method, the system assumes an initial index of NSNotFound and a length of `0`.

## See Also

### Getting the rows and columns

func accessibilityColumnRange() -> NSRange

Returns the columns spanned by the cell.

**Required**

