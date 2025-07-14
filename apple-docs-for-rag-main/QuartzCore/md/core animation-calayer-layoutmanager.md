

- Core Animation
- CALayer
-  layoutManager 

Instance Property

# layoutManager

The object responsible for laying out the layer’s sublayers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+

``` source
var layoutManager: (any CALayoutManager)? { get set }
```

## Discussion

The object you assign to this property must nominally implement the CALayoutManager Informal Protocol informal protocol. If the layer’s delegate does not handle layout updates, the object assigned to this property is given a chance to update the layout of the layer’s sublayers.

In macOS, assign an instance of the CAConstraintLayoutManager class to this property if your layer uses layer-based constraints to handle layout changes.

The default value of this property is `nil`.

## See Also

### Managing Layer Resizing and Layout

func setNeedsLayout()

Invalidates the layer’s layout and marks it as needing an update.

func layoutSublayers()

Tells the layer to update its layout.

func layoutIfNeeded()

Recalculate the receiver’s layout, if required.

func needsLayout() -> Bool

Returns a Boolean indicating whether the layer has been marked as needing a layout update.

var autoresizingMask: CAAutoresizingMask

A bitmask defining how the layer is resized when the bounds of its superlayer changes.

func resize(withOldSuperlayerSize: CGSize)

Informs the receiver that the size of its superlayer changed.

func resizeSublayers(withOldSize: CGSize)

Informs the receiver’s sublayers that the receiver’s size has changed.

func preferredFrameSize() -> CGSize

Returns the preferred size of the layer in the coordinate space of its superlayer.

