

- Core Animation
- CALayer
-  layoutSublayers() 

Instance Method

# layoutSublayers()

Tells the layer to update its layout.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func layoutSublayers()
```

## Discussion

Subclasses can override this method and use it to implement their own layout algorithm. Your implementation must set the frame of each sublayer managed by the receiver.

The default implementation of this method calls the `layoutSublayers(of:)` method in Swift or `layoutSublayersOfLayer:` method in Objective-C of the layer’s delegate object. If there is no delegate object, or the delegate does not implement that method, this method calls the `layoutSublayers(of:)` method in Swift or `layoutSublayersOfLayer:` method in Objective-C of the object in the layoutManager property.

## See Also

### Managing Layer Resizing and Layout

var layoutManager: (any CALayoutManager)?

The object responsible for laying out the layer’s sublayers.

func setNeedsLayout()

Invalidates the layer’s layout and marks it as needing an update.

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

