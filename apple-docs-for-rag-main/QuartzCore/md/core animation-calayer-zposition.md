

- Core Animation
- CALayer
-  zPosition 

Instance Property

# zPosition

The layer’s position on the z axis. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var zPosition: CGFloat { get set }
```

## Discussion

The default value of this property is `0`. Changing the value of this property changes the front-to-back ordering of layers onscreen. Higher values place this layer visually closer to the viewer than layers with lower values. This can affect the visibility of layers whose frame rectangles overlap.

The value of this property is measured in points. The range of this property is single-precision, floating-point `-`greatestFiniteMagnitude to greatestFiniteMagnitude.

## See Also

### Modifying the Layer Geometry

var frame: CGRect

The layer’s frame rectangle.

var bounds: CGRect

The layer’s bounds rectangle. Animatable.

var position: CGPoint

The layer’s position in its superlayer’s coordinate space. Animatable.

var anchorPointZ: CGFloat

The anchor point for the layer’s position along the z axis. Animatable.

var anchorPoint: CGPoint

Defines the anchor point of the layer’s bounds rectangle. Animatable.

var contentsScale: CGFloat

The scale factor applied to the layer.

