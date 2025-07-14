

- Core Animation
- CALayer
-  needsLayout() 

Instance Method

# needsLayout()

Returns a Boolean indicating whether the layer has been marked as needing a layout update.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func needsLayout() -> Bool
```

## Return Value

true if the layer has been marked as requiring a layout update.

## See Also

### Managing Layer Resizing and Layout

var layoutManager: (any CALayoutManager)?

The object responsible for laying out the layer’s sublayers.

func setNeedsLayout()

Invalidates the layer’s layout and marks it as needing an update.

func layoutSublayers()

Tells the layer to update its layout.

func layoutIfNeeded()

Recalculate the receiver’s layout, if required.

var autoresizingMask: CAAutoresizingMask

A bitmask defining how the layer is resized when the bounds of its superlayer changes.

func resize(withOldSuperlayerSize: CGSize)

Informs the receiver that the size of its superlayer changed.

func resizeSublayers(withOldSize: CGSize)

Informs the receiver’s sublayers that the receiver’s size has changed.

func preferredFrameSize() -> CGSize

Returns the preferred size of the layer in the coordinate space of its superlayer.

