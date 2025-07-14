

- AppKit
- NSRulerView
-  accessoryView 

Instance Property

# accessoryView

The receiver’s accessory view to `aView`.

macOS

``` source
@MainActor
var accessoryView: NSView? { get set }
```

## Discussion

Raises an `NSInternalInconsistencyException` if `aView` is not `nil` and the receiver has no client view.

## See Also

### Related Documentation

var reservedThicknessForAccessoryView: CGFloat

The room available for the receiver’s accessory view to `thickness`.

