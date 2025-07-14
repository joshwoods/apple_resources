

- Core Animation
- CALayer
-  setNeedsLayout() 

Instance Method

# setNeedsLayout()

Invalidates the layer’s layout and marks it as needing an update.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func setNeedsLayout()
```

## Discussion

You can call this method to indicate that the layout of a layer’s sublayers has changed and must be updated. The system typically calls this method automatically when the layer’s bounds change or when sublayers are added or removed. In macOS, if your layer’s layoutManager property contains an object that implements the `invalidateLayout(of:)` method in Swift or the `invalidateLayoutOfLayer:` method in Objective-C, the system calls that method too.

During the next update cycle, the system calls the layoutSublayers() method of any layers requiring layout updates.

## See Also

### Managing Layer Resizing and Layout

var layoutManager: (any CALayoutManager)?

The object responsible for laying out the layer’s sublayers.

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

