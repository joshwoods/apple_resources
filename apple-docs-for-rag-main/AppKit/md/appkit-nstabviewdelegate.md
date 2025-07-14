

- AppKit
-  NSTabViewDelegate 

Protocol

# NSTabViewDelegate

The `NSTabViewDelegate` protocol defines the optional methods implemented by delegates of `NSTabView` objects.

macOS

``` source
protocol NSTabViewDelegate : NSObjectProtocol
```

## Topics

### Adding and Removing Tabs

func tabViewDidChangeNumberOfTabViewItems(NSTabView)

Informs the delegate that the number of tab view items in `tabView` has changed.

### Selecting a Tab

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Invoked just before `tabViewItem` in `tabView` is selected.

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the delegate that `tabView` is about to select `tabViewItem`.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the delegate that `tabView` has selected `tabViewItem`.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTabViewController

## See Also

### Handling the Selection of Tabs

var delegate: (any NSTabViewDelegate)?

The tab view’s delegate.

