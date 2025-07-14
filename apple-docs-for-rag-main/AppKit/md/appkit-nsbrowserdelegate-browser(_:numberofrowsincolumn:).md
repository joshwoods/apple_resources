

- AppKit
- NSBrowserDelegate
-  browser(\_:numberOfRowsInColumn:) 

Instance Method

# browser(\_:numberOfRowsInColumn:)

Returns the number of rows of data in the specified column.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    numberOfRowsInColumn column: Int
) -> Int
```

## Parameters 

`sender`  

The browser.

`column`  

The index of the column.

## Return Value

The number of rows of data.

## Discussion

Either this method or browser(_:createRowsForColumn:in:) must be implemented, but not both.

## See Also

### Related Documentation

func browser(NSBrowser, willDisplayCell: Any, atRow: Int, column: Int)

Gives the delegate the opportunity to modify the specified cell at the given row and column location before the browser displays it.

### Getting Browser Information

func browser(NSBrowser, isColumnValid: Int) -> Bool

Returns whether the contents of the specified column are valid.

func browser(NSBrowser, numberOfChildrenOfItem: Any?) -> Int

Asks the delegate for the number of children the given item has.

func browser(NSBrowser, titleOfColumn: Int) -> String?

Asks the delegate for the title to display above the specified column.

