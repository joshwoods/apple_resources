

- AppKit
- NSBrowserDelegate
-  browser(\_:isColumnValid:) 

Instance Method

# browser(\_:isColumnValid:)

Returns whether the contents of the specified column are valid.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    isColumnValid column: Int
) -> Bool
```

## Parameters 

`sender`  

The browser containing the column to validate.

`column`  

The index of the column to validate.

## Return Value

true if the column’s contents are valid; otherwise, false. If false is returned, `sender` reloads the column.

## Discussion

This method is invoked in response to the validateVisibleColumns()method of NSBrowser being sent to `sender`.

## See Also

### Related Documentation

Browser Programming Topics

### Getting Browser Information

func browser(NSBrowser, numberOfRowsInColumn: Int) -> Int

Returns the number of rows of data in the specified column.

func browser(NSBrowser, numberOfChildrenOfItem: Any?) -> Int

Asks the delegate for the number of children the given item has.

func browser(NSBrowser, titleOfColumn: Int) -> String?

Asks the delegate for the title to display above the specified column.

