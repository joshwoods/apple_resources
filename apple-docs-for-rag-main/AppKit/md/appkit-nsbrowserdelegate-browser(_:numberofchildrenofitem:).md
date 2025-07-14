

- AppKit
- NSBrowserDelegate
-  browser(\_:numberOfChildrenOfItem:) 

Instance Method

# browser(\_:numberOfChildrenOfItem:)

Asks the delegate for the number of children the given item has.

macOS 10.6+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    numberOfChildrenOfItem item: Any?
) -> Int
```

## Parameters 

`browser`  

The browser.

`item`  

The item that has some number of children.

## Return Value

The number of children.

## See Also

### Getting Browser Information

func browser(NSBrowser, isColumnValid: Int) -> Bool

Returns whether the contents of the specified column are valid.

func browser(NSBrowser, numberOfRowsInColumn: Int) -> Int

Returns the number of rows of data in the specified column.

func browser(NSBrowser, titleOfColumn: Int) -> String?

Asks the delegate for the title to display above the specified column.

