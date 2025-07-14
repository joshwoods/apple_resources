

- Core Animation
- CALayer
-  render(in:) 

Instance Method

# render(in:)

Renders the layer and its sublayers into the specified context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func render(in ctx: CGContext)
```

## Parameters 

`ctx`  

The graphics context to use to render the layer.

## Discussion

This method renders directly from the layer tree, ignoring any animations added to the render tree. Renders in the coordinate space of the layer.

The following code shows how you can use render(in:) to create a UIImage from a CAShapeLayer with a path that describes a circle. After creating the layer, the code creates a CGContext into which the circle is rendered. After rendering, UIGraphicsGetImageFromCurrentImageContext() generates the image.

```
let diameter: CGFloat = 100
let rect = CGRect(origin: CGPoint.zero,
                  size: CGSize(width: diameter, height: diameter))

let shapeLayer = CAShapeLayer()
shapeLayer.fillColor = UIColor.white.cgColor
shapeLayer.lineWidth = 10
shapeLayer.path = CGPath(ellipseIn: rect,
                         transform: nil)

let renderer = UIGraphicsImageRenderer(size: rect.size)

let image = renderer.image {
    context in

    return shapeLayer.render(in: context.cgContext)
}

```

Important

The OS X v10.5 implementation of this method does not support the entire Core Animation composition model. `QCCompositionLayer`, `CAOpenGLLayer`, and `QTMovieLayer` layers are not rendered. Additionally, layers that use 3D transforms are not rendered, nor are layers that specify backgroundFilters, filters, compositingFilter, or a mask values. Future versions of macOS may add support for rendering these layers and properties.

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

var rasterizationScale: CGFloat

The scale at which to rasterize content, relative to the coordinate space of the layer. Animatable

var contentsFormat: CALayerContentsFormat

A hint for the desired storage format of the layer contents.

