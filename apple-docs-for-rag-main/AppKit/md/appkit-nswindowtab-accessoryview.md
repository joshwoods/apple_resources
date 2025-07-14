

- AppKit
- NSWindowTab
-  accessoryView 

Instance Property

# accessoryView

An optional accessory view for the tab.

macOS 10.13+

``` source
var accessoryView: NSView? { get set }
```

## Discussion

You can customize the window tab by adding an accessory view that displays alongside the tab’s title.

The translatesAutoresizingMaskIntoConstraints property is automatically set to false on the view. Constraints can be created and activated to specify the view’s width and height values. A constraint is automatically added to vertically center the view, and to right align the view within the tab.

