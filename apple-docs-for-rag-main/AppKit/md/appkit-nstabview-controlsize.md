

- AppKit
- NSTabView
-  controlSize 

Instance Property

# controlSize

The size of the tab view.

macOS

``` source
@MainActor
var controlSize: NSControl.ControlSize { get set }
```

## Discussion

The valid values for this property are described inControl Sizes in NSCell. The default value of this property is NSRegularControlSize.

## See Also

### Determining the Size

var minimumSize: NSSize

The minimum size necessary for the tab view to display tabs in a useful way.

var contentRect: NSRect

The rectangle describing the content area of the tab view.

