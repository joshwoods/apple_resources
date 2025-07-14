

- Core Animation
- CALayer
-  layoutIfNeeded() 

Instance Method

# layoutIfNeeded()

Recalculate the receiver’s layout, if required.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func layoutIfNeeded()
```

## Discussion

When this message is received, the layer’s super layers are traversed until a ancestor layer is found that does not require layout. Then layout is performed on the entire layer-tree beneath that ancestor.

## See Also

### Managing Layer Resizing and Layout

var layoutManager: (any CALayoutManager)?

The object responsible for laying out the layer’s sublayers.

func setNeedsLayout()

Invalidates the layer’s layout and marks it as needing an update.

func layoutSublayers()

Tells the layer to update its layout.

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

