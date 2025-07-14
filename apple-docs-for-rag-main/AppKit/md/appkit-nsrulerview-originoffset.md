

- AppKit
- NSRulerView
-  originOffset 

Instance Property

# originOffset

The distance to the zero hash mark from the bounds origin of the NSScrollView’s document view (not of the receiver’s client view), in the document view’s coordinate system.

macOS

``` source
@MainActor
var originOffset: CGFloat { get set }
```

## Discussion

The default offset is 0.0, meaning that the ruler origin coincides with the bounds origin of the document view.

