

- Core Animation
- CALayer
-  isGeometryFlipped 

Instance Property

# isGeometryFlipped

A Boolean that indicates whether the geometry of the layer and its sublayers is flipped vertically.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var isGeometryFlipped: Bool { get set }
```

## Discussion

If the layer is providing the backing for a layer-backed view, the view is responsible for managing the value in this property. For standalone layers, this property controls whether geometry values for the layer are interpreted using the standard or flipped coordinate system. The value of this property does not affect the rendering of the layer’s content.

The default value of this property is false.

## See Also

### Configuring the Layer’s Rendering Behavior

var isOpaque: Bool

A Boolean value indicating whether the layer contains completely opaque content.

var edgeAntialiasingMask: CAEdgeAntialiasingMask

A bitmask defining how the edges of the receiver are rasterized.

func contentsAreFlipped() -> Bool

Returns a Boolean indicating whether the layer content is implicitly flipped when rendered.

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

