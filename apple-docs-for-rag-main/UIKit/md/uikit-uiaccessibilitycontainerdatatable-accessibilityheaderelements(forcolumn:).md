

- UIKit
- UIAccessibilityContainerDataTable
-  accessibilityHeaderElements(forColumn:) 

Instance Method

# accessibilityHeaderElements(forColumn:)

Returns the accessibility element for the specified column header.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func accessibilityHeaderElements(forColumn column: Int) -> [any UIAccessibilityContainerDataTableCell]?
```

## Parameters 

`column`  

The index of the column containing the header.

## Return Value

The accessibility elements for the specified column header.

## See Also

### Providing header elements

func accessibilityHeaderElements(forRow: Int) -> [any UIAccessibilityContainerDataTableCell]?

Returns the accessibility element for the specified row header.

