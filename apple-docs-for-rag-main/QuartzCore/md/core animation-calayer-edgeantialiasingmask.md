

- Core Animation
- CALayer
-  edgeAntialiasingMask 

Instance Property

# edgeAntialiasingMask

A bitmask defining how the edges of the receiver are rasterized.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var edgeAntialiasingMask: CAEdgeAntialiasingMask { get set }
```

## Discussion

This property specifies which edges of the layer are antialiased and is a combination of the constants defined in CAEdgeAntialiasingMask. You can enable or disable antialiasing for each edge (top, left, bottom, right) separately. By default antialiasing is enabled for all edges.

Typically, you would use this property to disable antialiasing for edges that abut edges of other layers, to eliminate the seams that would otherwise occur.

## See Also

### Configuring the Layer’s Rendering Behavior

var isOpaque: Bool

A Boolean value indicating whether the layer contains completely opaque content.

func contentsAreFlipped() -> Bool

Returns a Boolean indicating whether the layer content is implicitly flipped when rendered.

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

