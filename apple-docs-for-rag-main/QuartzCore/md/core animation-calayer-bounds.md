

- Core Animation
- CALayer
-  bounds 

Instance Property

# bounds

The layer’s bounds rectangle. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var bounds: CGRect { get set }
```

## Discussion

The bounds rectangle is the origin and size of the layer in its own coordinate space. When you create a new standalone layer, the default value for this property is an empty rectangle, which you must change before using the layer. The values of each coordinate in the rectangle are measured in points.

For more information about the relationship between the frame, bounds, anchorPoint and position properties, see Core Animation Programming Guide.

## See Also

### Modifying the Layer Geometry

var frame: CGRect

The layer’s frame rectangle.

var position: CGPoint

The layer’s position in its superlayer’s coordinate space. Animatable.

var zPosition: CGFloat

The layer’s position on the z axis. Animatable.

var anchorPointZ: CGFloat

The anchor point for the layer’s position along the z axis. Animatable.

var anchorPoint: CGPoint

Defines the anchor point of the layer’s bounds rectangle. Animatable.

var contentsScale: CGFloat

The scale factor applied to the layer.

