

- AppKit
- NSScrubberFlowLayout
-  itemSize 

Instance Property

# itemSize

The frame size for each item in the scrubber.

macOS 10.12.2+

``` source
@MainActor
var itemSize: NSSize { get set }
```

## Discussion

You can override the value of this property on a per-item basis, by providing a delegate object to the scrubber that conforms to the NSScrubberFlowLayoutDelegate protocol. This delegate object must implement the scrubber(_:layout:sizeForItemAt:) method.

The default value for this property has a width of `50.0` points and a height of `30.0` points.

## See Also

### Configuring the layout

var itemSpacing: CGFloat

The horizontal spacing between items, specified in points.

