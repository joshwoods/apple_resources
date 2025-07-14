

- Core Animation
- CALayer
-  frame 

Instance Property

# frame

The layer’s frame rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var frame: CGRect { get set }
```

## Discussion

The frame rectangle is position and size of the layer specified in the superlayer’s coordinate space. For layers, the frame rectangle is a computed property that is derived from the values in thebounds, anchorPoint and position properties. When you assign a new value to this property, the layer changes its position and bounds properties to match the rectangle you specified. The values of each coordinate in the rectangle are measured in points.

Do not set the frame if the transform property applies a rotation transform that is not a multiple of 90 degrees.

For more information about the relationship between the frame, bounds, anchorPoint and position properties, see Core Animation Programming Guide.

Note

The `frame` property is not directly animatable. Instead you should animate the appropriate combination of the bounds, anchorPoint and position properties to achieve the desired result.

## See Also

### Modifying the Layer Geometry

var bounds: CGRect

The layer’s bounds rectangle. Animatable.

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

