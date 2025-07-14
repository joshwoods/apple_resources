

- AppKit
- NSBrowserDelegate
-  browser(\_:objectValueForItem:) 

Instance Method

# browser(\_:objectValueForItem:)

Returns the object that the specified item uses to draw its contents.

macOS 10.6+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    objectValueForItem item: Any?
) -> Any?
```

## Parameters 

`browser`  

The browser.

`item`  

The item in question.

## Return Value

The item’s object.

## See Also

### Accessing Components

func browser(NSBrowser, child: Int, ofItem: Any?) -> Any

Asks the delegate to return the child of the specified item at the specified index.

func browser(NSBrowser, isLeafItem: Any?) -> Bool

Asks the delegate whether the specified item is a leaf item (an item that cannot be expanded).

func browser(NSBrowser, shouldEditItem: Any?) -> Bool

Asks the delegate whether the browser may start an editing session for the specified item.

func browser(NSBrowser, setObjectValue: Any?, forItem: Any?)

Sets the object that the specified item uses to draw its contents to the specified object.

func rootItem(for: NSBrowser) -> Any?

Asks the delegate to return the root item of the browser.

func browser(NSBrowser, previewViewControllerForLeafItem: Any) -> NSViewController?

Asks the delegate for a controller that provides a preview column for the specified leaf item.

func browser(NSBrowser, headerViewControllerForItem: Any?) -> NSViewController?

Asks the delegate for a controller that provides a header view for the specified column item.

