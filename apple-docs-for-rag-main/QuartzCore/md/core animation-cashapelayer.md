

- Core Animation
-  CAShapeLayer 

Class

# CAShapeLayer

A layer that draws a cubic Bezier spline in its coordinate space.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CAShapeLayer
```

## Overview

The shape is composited between the layer’s contents and its first sublayer.

The shape will be drawn antialiased, and whenever possible it will be mapped into screen space before being rasterized to preserve resolution independence. However, certain kinds of image processing operations, such as CoreImage filters, applied to the layer or its ancestors may force rasterization in a local coordinate space.

The following code shows how you can build complex, composite paths and display them using a shape layer. In this example, a series of progressively transformed ellipses form a simple flower shape. The shape layer that displays the path has its fillRule set to evenOdd which stops the overlapping “petals” from filling with the yellow fillColor.

```
let width: CGFloat = 640
let height: CGFloat = 640

let shapeLayer = CAShapeLayer()
shapeLayer.frame = CGRect(x: 0, y: 0,
                          width: width, height: height)

let path = CGMutablePath()

stride(from: 0, to: CGFloat.pi * 2, by: CGFloat.pi / 6).forEach {
    angle in 
    var transform  = CGAffineTransform(rotationAngle: angle)
        .concatenating(CGAffineTransform(translationX: width / 2, y: height / 2))

    let petal = CGPath(ellipseIn: CGRect(x: -20, y: 0, width: 40, height: 100),
                       transform: &transform)

    path.addPath(petal)
}

shapeLayer.path = path
shapeLayer.strokeColor = UIColor.red.cgColor
shapeLayer.fillColor = UIColor.yellow.cgColor
shapeLayer.fillRule = kCAFillRuleEvenOdd
```

The following figure shows the resulting shape layer.

Note

Shape rasterization may favor speed over accuracy. For example, pixels with multiple intersecting path segments may not give exact results.

## Topics

### Specifying the Shape Path

var path: CGPath?

The path defining the shape to be rendered. Animatable.

### Accessing Shape Style Properties

var fillColor: CGColor?

The color used to fill the shape’s path. Animatable.

var fillRule: CAShapeLayerFillRule

The fill rule used when filling the shape’s path.

var lineCap: CAShapeLayerLineCap

Specifies the line cap style for the shape’s path.

var lineDashPattern: [NSNumber]?

The dash pattern applied to the shape’s path when stroked.

var lineDashPhase: CGFloat

The dash phase applied to the shape’s path when stroked. Animatable.

var lineJoin: CAShapeLayerLineJoin

Specifies the line join style for the shape’s path.

var lineWidth: CGFloat

Specifies the line width of the shape’s path. Animatable.

var miterLimit: CGFloat

The miter limit used when stroking the shape’s path. Animatable.

var strokeColor: CGColor?

The color used to stroke the shape’s path. Animatable.

var strokeStart: CGFloat

The relative location at which to begin stroking the path. Animatable.

var strokeEnd: CGFloat

The relative location at which to stop stroking the path. Animatable.

### Constants

Shape Fill Mode Values

These constants specify the possible fill modes for fillRule.

Line Join Values

These constants specify the shape of the joints between connected segments of a stroked path.

Line Cap Values

These constants specify the shape of endpoints for an open path when stroked.

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

class CAGradientLayer

A layer that draws a color gradient over its background color, filling the shape of the layer.

