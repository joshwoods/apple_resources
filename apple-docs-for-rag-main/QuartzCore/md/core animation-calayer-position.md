

- Core Animation
- CALayer
-  position 

Instance Property

# position

The layer’s position in its superlayer’s coordinate space. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var position: CGPoint { get set }
```

## Discussion

The value of this property is specified in points and is always specified relative to the value in the anchorPoint property. For new standalone layers, the default position is set to (0.0, 0.0). Changing the frame property also updates the value in this property.

For more information about the relationship between the frame, bounds, anchorPoint and position properties, see Core Animation Programming Guide.

## See Also

### Modifying the Layer Geometry

var frame: CGRect

The layer’s frame rectangle.

var bounds: CGRect

The layer’s bounds rectangle. Animatable.

var zPosition: CGFloat

The layer’s position on the z axis. Animatable.

var anchorPointZ: CGFloat

The anchor point for the layer’s position along the z axis. Animatable.

var anchorPoint: CGPoint

Defines the anchor point of the layer’s bounds rectangle. Animatable.

var contentsScale: CGFloat

The scale factor applied to the layer.

