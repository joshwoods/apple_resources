

- Core Animation
- CALayer
-  resize(withOldSuperlayerSize:) 

Instance Method

# resize(withOldSuperlayerSize:)

Informs the receiver that the size of its superlayer changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+

``` source
func resize(withOldSuperlayerSize size: CGSize)
```

## Parameters 

`size`  

The previous size of the superlayer.

## Discussion

When the autoresizingMask property is used for resizing and the bounds of a layer change, that layer calls this method on each of its sublayers. Sublayers use this method to adjust their own frame rectangles to reflect the new superlayer bounds, which can be retrieved directly from the superlayer. The old size of the superlayer is passed to this method so that the sublayer has that information for any calculations it must make.

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

func needsLayout() -> Bool

Returns a Boolean indicating whether the layer has been marked as needing a layout update.

var autoresizingMask: CAAutoresizingMask

A bitmask defining how the layer is resized when the bounds of its superlayer changes.

func resizeSublayers(withOldSize: CGSize)

Informs the receiver’s sublayers that the receiver’s size has changed.

func preferredFrameSize() -> CGSize

Returns the preferred size of the layer in the coordinate space of its superlayer.

