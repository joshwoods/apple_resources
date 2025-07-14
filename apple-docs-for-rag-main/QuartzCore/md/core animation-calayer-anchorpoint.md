

- Core Animation
- CALayer
-  anchorPoint 

Instance Property

# anchorPoint

Defines the anchor point of the layer’s bounds rectangle. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var anchorPoint: CGPoint { get set }
```

## Discussion

You specify the value for this property using the unit coordinate space. The default value of this property is (0.5, 0.5), which represents the center of the layer’s bounds rectangle. All geometric manipulations to the view occur about the specified point. For example, applying a rotation transform to a layer with the default anchor point causes the layer to rotate around its center. Changing the anchor point to a different location would cause the layer to rotate around that new point.

For more information about the relationship between the frame, bounds, anchorPoint and position properties, see Core Animation Programming Guide.

## See Also

### Modifying the Layer Geometry

var frame: CGRect

The layer’s frame rectangle.

var bounds: CGRect

The layer’s bounds rectangle. Animatable.

var position: CGPoint

The layer’s position in its superlayer’s coordinate space. Animatable.

var zPosition: CGFloat

The layer’s position on the z axis. Animatable.

var anchorPointZ: CGFloat

The anchor point for the layer’s position along the z axis. Animatable.

var contentsScale: CGFloat

The scale factor applied to the layer.

