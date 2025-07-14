

- WatchKit
- WKInterfaceDevice
-  screenScale 

Instance Property

# screenScale

The number of pixels per point for the current screen.

watchOS 2.0+

``` source
var screenScale: CGFloat { get }
```

## Discussion

The screen scale value applies to both the vertical and horizontal dimensions. For Apple Watch, this value is `2.0`.

## See Also

### Reading the Screen Information

var screenBounds: CGRect

The bounding rectangle of the screen.

