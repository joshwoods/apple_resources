

- Core Animation
- CALayer
-  contentsAreFlipped() 

Instance Method

# contentsAreFlipped()

Returns a Boolean indicating whether the layer content is implicitly flipped when rendered.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func contentsAreFlipped() -> Bool
```

## Return Value

true if the layer contents are implicitly flipped when rendered or false if they are not. This method returns false by default.

## Discussion

This method provides information about whether the layer’s contents are being flipped during drawing. You should not attempt to override this method and return a different value.

If the layer needs to flip its content, it returns true from this method and applies a y-flip transform to the graphics context before passing it to the layer’s draw(in:) method. Similarly, the layer converts any rectangles passed to its setNeedsDisplay(_:) into the flipped coordinate space.

## See Also

### Configuring the Layer’s Rendering Behavior

var isOpaque: Bool

A Boolean value indicating whether the layer contains completely opaque content.

var edgeAntialiasingMask: CAEdgeAntialiasingMask

A bitmask defining how the edges of the receiver are rasterized.

var isGeometryFlipped: Bool

A Boolean that indicates whether the geometry of the layer and its sublayers is flipped vertically.

var drawsAsynchronously: Bool

A Boolean indicating whether drawing commands are deferred and processed asynchronously in a background thread.

var shouldRasterize: Bool

A Boolean that indicates whether the layer is rendered as a bitmap before compositing. Animatable

var rasterizationScale: CGFloat

The scale at which to rasterize content, relative to the coordinate space of the layer. Animatable

var contentsFormat: CALayerContentsFormat

A hint for the desired storage format of the layer contents.

func render(in: CGContext)

Renders the layer and its sublayers into the specified context.

