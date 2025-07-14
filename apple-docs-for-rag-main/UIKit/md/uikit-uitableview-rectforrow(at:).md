

- UIKit
- UITableView
-  rectForRow(at:) 

Instance Method

# rectForRow(at:)

Returns the drawing area for a row that an index path identifies.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func rectForRow(at indexPath: IndexPath) -> CGRect
```

## Parameters 

`indexPath`  

An index path object that identifies a row by its index and its section index.

## Return Value

A rectangle defining the area in which the table view draws the row or CGRectZero if `indexPath` is invalid.

## See Also

### Getting the drawing areas for the table

func rect(forSection: Int) -> CGRect

Returns the drawing area for a specified section of the table view.

func rectForFooter(inSection: Int) -> CGRect

Returns the drawing area for the footer of the specified section.

func rectForHeader(inSection: Int) -> CGRect

Returns the drawing area for the header of the specified section.

