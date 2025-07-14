

- UIKit
-  UIAccessibilityContainerDataTableCell 

Protocol

# UIAccessibilityContainerDataTableCell

Methods that provide the location of a cell in a table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
protocol UIAccessibilityContainerDataTableCell : NSObjectProtocol
```

## Topics

### Getting the rows and columns

func accessibilityColumnRange() -> NSRange

Returns the columns spanned by the cell.

**Required**

func accessibilityRowRange() -> NSRange

Returns the visible range of rows.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Containers

protocol UIAccessibilityContainerDataTable

Methods that convey information about the contents of a table.

enum UIAccessibilityContainerType

Constants that indicate the type of content in a data-based container.

