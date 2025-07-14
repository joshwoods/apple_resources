

- AppKit
- NSBrowserDelegate
-  browser(\_:previewViewControllerForLeafItem:) 

Instance Method

# browser(\_:previewViewControllerForLeafItem:)

Asks the delegate for a controller that provides a preview column for the specified leaf item.

macOS 10.6+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    previewViewControllerForLeafItem item: Any
) -> NSViewController?
```

## Parameters 

`browser`  

The browser.

`item`  

The leaf item.

## Return Value

A view controller that provides a preview column, or `nil` to suppress the preview column.

## Discussion

The returned controller’s represented object is set to the specified leaf item. This method is called only if the delegate implements the item data source methods.

## See Also

### Accessing Components

func browser(NSBrowser, child: Int, ofItem: Any?) -> Any

Asks the delegate to return the child of the specified item at the specified index.

func browser(NSBrowser, isLeafItem: Any?) -> Bool

Asks the delegate whether the specified item is a leaf item (an item that cannot be expanded).

func browser(NSBrowser, shouldEditItem: Any?) -> Bool

Asks the delegate whether the browser may start an editing session for the specified item.

func browser(NSBrowser, objectValueForItem: Any?) -> Any?

Returns the object that the specified item uses to draw its contents.

func browser(NSBrowser, setObjectValue: Any?, forItem: Any?)

Sets the object that the specified item uses to draw its contents to the specified object.

func rootItem(for: NSBrowser) -> Any?

Asks the delegate to return the root item of the browser.

func browser(NSBrowser, headerViewControllerForItem: Any?) -> NSViewController?

Asks the delegate for a controller that provides a header view for the specified column item.

