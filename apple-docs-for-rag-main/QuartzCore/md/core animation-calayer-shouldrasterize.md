

- Core Animation
- CALayer
-  shouldRasterize 

Instance Property

# shouldRasterize

A Boolean that indicates whether the layer is rendered as a bitmap before compositing. Animatable

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var shouldRasterize: Bool { get set }
```

## Discussion

When the value of this property is true, the layer is rendered as a bitmap in its local coordinate space and then composited to the destination with any other content. Shadow effects and any filters in the filters property are rasterized and included in the bitmap. However, the current opacity of the layer is not rasterized. If the rasterized bitmap requires scaling during compositing, the filters in the minificationFilter and magnificationFilter properties are applied as needed.

When the value of this property is false, the layer is composited directly into the destination whenever possible. The layer may still be rasterized prior to compositing if certain features of the compositing model (such as the inclusion of filters) require it.

The default value of this property is false.

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

var rasterizationScale: CGFloat

The scale at which to rasterize content, relative to the coordinate space of the layer. Animatable

var contentsFormat: CALayerContentsFormat

A hint for the desired storage format of the layer contents.

func render(in: CGContext)

Renders the layer and its sublayers into the specified context.

