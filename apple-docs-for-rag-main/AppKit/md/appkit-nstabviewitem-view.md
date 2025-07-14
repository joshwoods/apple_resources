

- AppKit
- NSTabViewItem
-  view 

Instance Property

# view

Sets the view associated with the receiver to `view`.

macOS

``` source
var view: NSView? { get set }
```

## Discussion

This is the view displayed when a user clicks the tab. When you set a new view, the old view is released.

