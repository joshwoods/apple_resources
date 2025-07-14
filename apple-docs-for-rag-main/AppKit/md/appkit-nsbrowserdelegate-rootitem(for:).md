

- AppKit
- NSBrowserDelegate
-  rootItem(for:) 

Instance Method

# rootItem(for:)

Asks the delegate to return the root item of the browser.

macOS 10.6+

``` source
@MainActor
optional func rootItem(for browser: NSBrowser) -> Any?
```

## Parameters 

`browser`  

The browser.

## Return Value

The browser’s root item.

## Discussion

By default, `nil` identifies the root item. This method can specify a different root item. To reload the previously set root item, call loadColumnZero(), and rootItem(for:) will be called again.

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

func browser(NSBrowser, previewViewControllerForLeafItem: Any) -> NSViewController?

Asks the delegate for a controller that provides a preview column for the specified leaf item.

func browser(NSBrowser, headerViewControllerForItem: Any?) -> NSViewController?

Asks the delegate for a controller that provides a header view for the specified column item.

