

- Core Animation
- CALayer
-  rasterizationScale 

Instance Property

# rasterizationScale

The scale at which to rasterize content, relative to the coordinate space of the layer. Animatable

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var rasterizationScale: CGFloat { get set }
```

## Discussion

When the value in the shouldRasterize property is true, the layer uses this property to determine whether to scale the rasterized content (and by how much). The default value of this property is `1.0`, which indicates that the layer should be rasterized at its current size. Larger values magnify the content and smaller values shrink it.

## See Also

### Configuring the Layer’s Rendering Behavior

var isOpaque: Bool

A Boolean value indicating whether the layer contains completely opaque content.

var edgeAntialiasingMask: CAEdgeAntialiasingMask

A bitmask defining how the edges of the receiver are rasterized.

func contentsAreFlipped() -> Bool

Returns a Boolean indicating whether the layer content is implicitly flipped when rendered.

var isGeometryFlipped: Bool

A Boolean that indicates whether the geometry of the layer and its sublayers is flipped vertically.

var drawsAsynchronously: Bool

A Boolean indicating whether drawing commands are deferred and processed asynchronously in a background thread.

var shouldRasterize: Bool

A Boolean that indicates whether the layer is rendered as a bitmap before compositing. Animatable

var contentsFormat: CALayerContentsFormat

A hint for the desired storage format of the layer contents.

func render(in: CGContext)

Renders the layer and its sublayers into the specified context.

