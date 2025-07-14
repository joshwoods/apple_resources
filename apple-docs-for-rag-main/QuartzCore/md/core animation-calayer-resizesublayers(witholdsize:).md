

- Core Animation
- CALayer
-  resizeSublayers(withOldSize:) 

Instance Method

# resizeSublayers(withOldSize:)

Informs the receiver’s sublayers that the receiver’s size has changed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+

``` source
func resizeSublayers(withOldSize size: CGSize)
```

## Parameters 

`size`  

The previous size of the current layer.

## Discussion

When the autoresizingMask property is used for resizing and the bounds of this layer change, the layer calls this method. The default implementation calls the resize(withOldSuperlayerSize:) method of each sublayer to let it know its superlayer’s bounds changed. You should not need to call or override this method directly.

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

func resize(withOldSuperlayerSize: CGSize)

Informs the receiver that the size of its superlayer changed.

func preferredFrameSize() -> CGSize

Returns the preferred size of the layer in the coordinate space of its superlayer.

