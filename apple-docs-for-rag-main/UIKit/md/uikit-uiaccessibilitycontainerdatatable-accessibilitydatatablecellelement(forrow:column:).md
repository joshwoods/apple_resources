

- UIKit
- UIAccessibilityContainerDataTable
-  accessibilityDataTableCellElement(forRow:column:) 

Instance Method

# accessibilityDataTableCellElement(forRow:column:)

Returns the accessibility element for the specified cell.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func accessibilityDataTableCellElement(
    forRow row: Int,
    column: Int
) -> (any UIAccessibilityContainerDataTableCell)?
```

**Required**

## Parameters 

`row`  

The row of the cell.

`column`  

The column of the cell.

## Return Value

The accessibility element for the cell.

