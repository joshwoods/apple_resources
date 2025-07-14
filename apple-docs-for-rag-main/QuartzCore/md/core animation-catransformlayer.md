

- Core Animation
-  CATransformLayer 

Class

# CATransformLayer

Objects used to create true 3D layer hierarchies, rather than the flattened hierarchy rendering model used by other layer types.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CATransformLayer
```

## Overview

Unlike normal layers, transform layers do not flatten their sublayers into the plane at `Z=0`. Due to this, they do not support many of the features of the `CALayer` class compositing model:

- Only the sublayers of a transform layer are rendered. The `CALayer` properties that are rendered by a layer are ignored, including: `backgroundColor`, `contents`, border style properties, stroke style properties, etc.

- The properties that assume 2D image processing are also ignored, including: `filters`, `backgroundFilters`, `compositingFilter`, `mask`, `masksToBounds`, and shadow style properties.

- The `opacity` property is applied to each sublayer individually, the transform layer does not form a compositing group.

- The hitTest(_:) method should never be called on a transform layer as they do not have a 2D coordinate space into which the point can be mapped.

### Example: Displaying layers in 3D

Because CATransformLayer creates true 3D layer hierarchies, you can display otherwise hidden layers when applying 3D transforms.

The following code shows three layers with different colors but identical sizes added at the same position to `layer`. The blue layer is visible because it has the highest zPosition. Defining the layer’s transform rotates the viewpoint in 3D space and, because `layer` is a CATransformLayer, all three layers are visible as illustrated below.

```
let layer = CATransformLayer()

func layerOfColor(_ color: UIColor, zPosition: CGFloat) -> CALayer {
    let layer = CALayer()
    layer.frame = CGRect(x: 200, y: -200, width: 400, height: 400)
    layer.backgroundColor = color.cgColor
    layer.zPosition = zPosition
    layer.opacity = 0.5

    return layer
}

layer.addSublayer(layerOfColor(.red, zPosition: 20))
layer.addSublayer(layerOfColor(.green, zPosition: 40))
layer.addSublayer(layerOfColor(.blue, zPosition: 60))

var perspective = CATransform3DIdentity
perspective.m34 = -1 / 100

layer.transform = CATransform3DRotate(perspective, 0.1, 0, 1, 0)
```

However, if `layer` is created as a CALayer, the green and red layers, being hidden by the blue layer, are not rendered as illustrated in the following figure.

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

### Advanced Layer Options

class CAScrollLayer

A layer that displays scrollable content larger than its own bounds.

class CATiledLayer

A layer that provides a way to asynchronously provide tiles of the layer’s content, potentially cached at multiple levels of detail.

class CAReplicatorLayer

A layer that creates a specified number of sublayer copies with varying geometric, temporal, and color transformations.

