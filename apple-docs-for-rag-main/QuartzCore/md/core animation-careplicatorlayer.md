

- Core Animation
-  CAReplicatorLayer 

Class

# CAReplicatorLayer

A layer that creates a specified number of sublayer copies with varying geometric, temporal, and color transformations.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
class CAReplicatorLayer
```

## Overview

You can use a CAReplicatorLayer object to build complex layouts based on a single source layer that is replicated with transformation rules that can affect the position, rotation color, and time.

The following shows a simple example: a red square is added to a replicator layer with an instance count of `5`. The position of each replicated instance is offset along the `x` axis so that it appears to the right of the previous instance. The blue and green color channels are offset so that their values reach `0` at the final instance.

```
let replicatorLayer = CAReplicatorLayer()

let redSquare = CALayer()
redSquare.backgroundColor = NSColor.white.cgColor
redSquare.frame = CGRect(x: 0, y: 0, width: 100, height: 100)

let instanceCount = 5

replicatorLayer.instanceCount = instanceCount
replicatorLayer.instanceTransform = CATransform3DMakeTranslation(110, 0, 0)

let offsetStep = -1 / Float(instanceCount)
replicatorLayer.instanceBlueOffset = offsetStep
replicatorLayer.instanceGreenOffset = offsetStep

replicatorLayer.addSublayer(redSquare)
```

The result of the code above is a row of five squares, with colors graduating from white to red.

Replicator layers can be nested. The following code adds `replicatorLayer` to a second replicator layer that offsets the position of each instance vertically and subtracts from the red channel.

```
let outerReplicatorLayer = CAReplicatorLayer()

outerReplicatorLayer.addSublayer(replicatorLayer)

outerReplicatorLayer.instanceCount = instanceCount
outerReplicatorLayer.instanceTransform = CATransform3DMakeTranslation(0, 110, 0)
outerReplicatorLayer.instanceRedOffset = offsetStep
```

The result of adding this code is to create a grid with the value of the red channel being reduced in the vertical direction.

Note

The CAReplicatorLayer implementation of hitTest(_:) currently tests only the first instance of z replicator layer’s sublayers. This may change in the future.

## Topics

### Setting Instance Display Properties

var instanceCount: Int

The number of copies to create, including the source layers.

var instanceDelay: CFTimeInterval

Specifies the delay, in seconds, between replicated copies. Animatable.

var instanceTransform: CATransform3D

The transform matrix applied to the previous instance to produce the current instance. Animatable.

### Modifying Instance Layer Geometry

var preservesDepth: Bool

Defines whether this layer flattens its sublayers into its plane.

### Accessing Instance Color Values

var instanceColor: CGColor?

Defines the color used to multiply the source object. Animatable.

var instanceRedOffset: Float

Defines the offset added to the red component of the color for each replicated instance. Animatable.

var instanceGreenOffset: Float

Defines the offset added to the green component of the color for each replicated instance. Animatable.

var instanceBlueOffset: Float

Defines the offset added to the blue component of the color for each replicated instance. Animatable.

var instanceAlphaOffset: Float

Defines the offset added to the alpha component of the color for each replicated instance. Animatable.

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

class CATransformLayer

Objects used to create true 3D layer hierarchies, rather than the flattened hierarchy rendering model used by other layer types.

