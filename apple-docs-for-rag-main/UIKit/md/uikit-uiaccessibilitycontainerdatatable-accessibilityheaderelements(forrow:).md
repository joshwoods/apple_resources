

- UIKit
- UIAccessibilityContainerDataTable
-  accessibilityHeaderElements(forRow:) 

Instance Method

# accessibilityHeaderElements(forRow:)

Returns the accessibility element for the specified row header.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
optional func accessibilityHeaderElements(forRow row: Int) -> [any UIAccessibilityContainerDataTableCell]?
```

## Parameters 

`row`  

The index of the row containing the header.

## Return Value

The accessibility elements for the specified row header.

## See Also

### Providing header elements

func accessibilityHeaderElements(forColumn: Int) -> [any UIAccessibilityContainerDataTableCell]?

Returns the accessibility element for the specified column header.

