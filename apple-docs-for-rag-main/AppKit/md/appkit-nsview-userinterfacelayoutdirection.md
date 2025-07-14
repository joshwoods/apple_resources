

- AppKit
- NSView
-  userInterfaceLayoutDirection 

Instance Property

# userInterfaceLayoutDirection

The layout direction for content in the view.

macOS 10.8+

``` source
@MainActor
var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection { get set }
```

## Discussion

Different languages support different directions for laying out content. While many languages support left-to-right layout, some support right-to-left layout. This property contains the preferred layout direction employed by the view. It is the responsibility of the view to respect this value and lay out its content appropriately.

In macOS 10.9 and later, if no layout direction is set explicitly, this property contains the value reported by the app’s userInterfaceLayoutDirection property. In prior versions of macOS, it returns the value NSUserInterfaceLayoutDirection.leftToRight by default. Certain AppKit subclasses, such as NSOutlineView, respect the value returned by this method and adjust their layout accordingly.

