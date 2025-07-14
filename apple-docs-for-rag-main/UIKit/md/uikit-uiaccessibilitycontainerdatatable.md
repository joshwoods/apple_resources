

- UIKit
-  UIAccessibilityContainerDataTable 

Protocol

# UIAccessibilityContainerDataTable

Methods that convey information about the contents of a table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
protocol UIAccessibilityContainerDataTable : NSObjectProtocol
```

## Topics

### Providing cell elements

func accessibilityDataTableCellElement(forRow: Int, column: Int) -> (any UIAccessibilityContainerDataTableCell)?

Returns the accessibility element for the specified cell.

**Required**

### Providing the table dimensions

func accessibilityColumnCount() -> Int

Returns the total number of columns in the table.

**Required**

func accessibilityRowCount() -> Int

Returns the total number of rows in the table.

**Required**

### Providing header elements

func accessibilityHeaderElements(forColumn: Int) -> [any UIAccessibilityContainerDataTableCell]?

Returns the accessibility element for the specified column header.

func accessibilityHeaderElements(forRow: Int) -> [any UIAccessibilityContainerDataTableCell]?

Returns the accessibility element for the specified row header.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Containers

protocol UIAccessibilityContainerDataTableCell

Methods that provide the location of a cell in a table.

enum UIAccessibilityContainerType

Constants that indicate the type of content in a data-based container.

