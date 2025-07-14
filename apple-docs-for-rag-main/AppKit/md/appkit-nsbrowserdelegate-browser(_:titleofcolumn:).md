

- AppKit
- NSBrowserDelegate
-  browser(\_:titleOfColumn:) 

Instance Method

# browser(\_:titleOfColumn:)

Asks the delegate for the title to display above the specified column.

macOS

``` source
@MainActor
optional func browser(
    _ sender: NSBrowser,
    titleOfColumn column: Int
) -> String?
```

## Parameters 

`sender`  

The browser.

`column`  

The index the column to be titled.

## Return Value

The title of the specified column.

## See Also

### Related Documentation

func setTitle(String, ofColumn: Int)

Sets the title of the given column.

func title(ofColumn: Int) -> String?

Returns the title displayed for the given column.

### Getting Browser Information

func browser(NSBrowser, isColumnValid: Int) -> Bool

Returns whether the contents of the specified column are valid.

func browser(NSBrowser, numberOfRowsInColumn: Int) -> Int

Returns the number of rows of data in the specified column.

func browser(NSBrowser, numberOfChildrenOfItem: Any?) -> Int

Asks the delegate for the number of children the given item has.

