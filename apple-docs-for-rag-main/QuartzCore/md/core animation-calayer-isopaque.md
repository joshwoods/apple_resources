

- Core Animation
- CALayer
-  isOpaque 

Instance Property

# isOpaque

A Boolean value indicating whether the layer contains completely opaque content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var isOpaque: Bool { get set }
```

## Discussion

The default value of this property is false. If your app draws completely opaque content that fills the layer’s bounds, setting this property to true lets the system optimize the rendering behavior for the layer. Specifically, when the layer creates the backing store for your drawing commands, Core Animation omits the alpha channel of that backing store. Doing so can improve the performance of compositing operations. If you set the value of this property to true, you must fill the layer’s bounds with opaque content.

Setting this property affects only the backing store managed by Core Animation. If you assign an image with an alpha channel to the layer’s contents property, that image retains its alpha channel regardless of the value of this property.

## See Also

### Configuring the Layer’s Rendering Behavior

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

var rasterizationScale: CGFloat

The scale at which to rasterize content, relative to the coordinate space of the layer. Animatable

var contentsFormat: CALayerContentsFormat

A hint for the desired storage format of the layer contents.

func render(in: CGContext)

Renders the layer and its sublayers into the specified context.

