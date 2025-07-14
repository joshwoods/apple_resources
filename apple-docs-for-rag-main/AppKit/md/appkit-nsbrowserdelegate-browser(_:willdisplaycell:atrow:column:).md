

- AppKit
- NSBrowserDelegate
-  browser(\_:willDisplayCell:atRow:column:) 

Instance Method

# browser(\_:willDisplayCell:atRow:column:)

Gives the delegate the opportunity to modify the specified cell at the given row and column location before the browser displays it.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    willDisplayCell cell: Any,
    atRow row: Int,
    column: Int
)
```

## Parameters 

`sender`  

The browser.

`cell`  

The cell to be displayed.

`row`  

The row index of the cell to be displayed.

`column`  

The column index of the cell to be displayed.

## Discussion

The delegate should set any state necessary for the correct display of the cell.

## See Also

### Related Documentation

func browser(NSBrowser, numberOfRowsInColumn: Int) -> Int

Returns the number of rows of data in the specified column.

### Managing Columns

func browser(NSBrowser, createRowsForColumn: Int, in: NSMatrix)

Creates a row in the given matrix for each row of data in the specified column of the browser.

func browser(NSBrowser, didChangeLastColumn: Int, toColumn: Int)

Tells the delegate that the browser’s last column changed.

