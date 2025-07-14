

- Core Animation
-  CAGradientLayer 

Class

# CAGradientLayer

A layer that draws a color gradient over its background color, filling the shape of the layer.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CAGradientLayer
```

## Overview

You use a gradient layer to create a color gradient containing an arbitrary number of colors. By default, the colors are spread uniformly across the layer, but you can optionally specify locations for control over the color positions through the gradient.

The following code shows how to create a gradient layer containing four colors that are evenly distributed through the gradient. Rotating the layer by 90° (doc://com.apple.documentation/documentation/corefoundation/cgfloat/1845230-pi `/ 2` radians) gives a horizontal gradient.

```
gradientLayer.colors = [UIColor.red.cgColor,
                        UIColor.yellow.cgColor,
                        UIColor.green.cgColor,
                        UIColor.blue.cgColor]

gradientLayer.transform = CATransform3DMakeRotation(CGFloat.pi / 2, 0, 0, 1)
```

The following figure shows the appearance of the gradient layer.

## Topics

### Gradient Style Properties

var colors: [Any]?

An array of `CGColorRef` objects defining the color of each gradient stop. Animatable.

var locations: [NSNumber]?

An optional array of NSNumber objects defining the location of each gradient stop. Animatable.

var endPoint: CGPoint

The end point of the gradient when drawn in the layer’s coordinate space. Animatable.

var startPoint: CGPoint

The start point of the gradient when drawn in the layer’s coordinate space. Animatable.

var type: CAGradientLayerType

Style of gradient drawn by the layer.

### Constants

Gradient Types

The style of gradient drawn by the layer.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Text, Shapes, and Gradients

class CATextLayer

A layer that provides simple text layout and rendering of plain or attributed strings.

class CAShapeLayer

A layer that draws a cubic Bezier spline in its coordinate space.

