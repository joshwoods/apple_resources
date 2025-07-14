

- AppKit
- NSBrowserDelegate
-  browser(\_:createRowsForColumn:in:) 

Instance Method

# browser(\_:createRowsForColumn:in:)

Creates a row in the given matrix for each row of data in the specified column of the browser.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    createRowsForColumn column: Int,
    in matrix: NSMatrix
)
```

## Parameters 

`sender`  

The browser.

`column`  

The index of the column in which the rows are located.

`matrix`  

The matrix in which the rows are created.

## Discussion

Either this method or browser(_:numberOfRowsInColumn:) must be implemented, but not both, or an NSBrowserIllegalDelegateException will be raised.

## See Also

### Managing Columns

func browser(NSBrowser, willDisplayCell: Any, atRow: Int, column: Int)

Gives the delegate the opportunity to modify the specified cell at the given row and column location before the browser displays it.

func browser(NSBrowser, didChangeLastColumn: Int, toColumn: Int)

Tells the delegate that the browser’s last column changed.

