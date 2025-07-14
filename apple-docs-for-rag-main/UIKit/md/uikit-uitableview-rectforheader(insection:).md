

- UIKit
- UITableView
-  rectForHeader(inSection:) 

Instance Method

# rectForHeader(inSection:)

Returns the drawing area for the header of the specified section.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func rectForHeader(inSection section: Int) -> CGRect
```

## Parameters 

`section`  

An index number identifying a section of the table view. Plain-style table views always have a section index of zero.

## Return Value

A rectangle defining the area in which the table view draws the section header.

## See Also

### Getting the drawing areas for the table

func rect(forSection: Int) -> CGRect

Returns the drawing area for a specified section of the table view.

func rectForRow(at: IndexPath) -> CGRect

Returns the drawing area for a row that an index path identifies.

func rectForFooter(inSection: Int) -> CGRect

Returns the drawing area for the footer of the specified section.

