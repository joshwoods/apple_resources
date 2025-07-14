

- SceneKit
-  SCNMorpher 

Class

# SCNMorpher

An object that manages smooth transitions between a node’s base geometry and one or more target geometries.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNMorpher
```

## Overview

You control these transitions by associating an SCNMorpher object with a node using its morpher property. The morpher maintains an array of target geometries and a set of weights associated with each. When all weights are zero, the surface takes the form of the base geometry (from the node’s geometry property). When you use the setWeight(_:forTargetAt:) method to increase a weight to `1.0`, the surface takes the form of the geometry at the corresponding index in the morpher’s targets array. If you use a variety of weight values for several targets, the surface takes a form that proportionally interpolates between the target geometries.

You can also animate weights implicitly or explicitly using keypath animations. For example, the following code creates a morph animation that transitions one target weight back and forth repeatedly:

```
CABasicAnimation *animation = [CABasicAnimation animationWithKeyPath:@"morpher.weights[0]"];
animation.fromValue = @0.0;
animation.toValue = @1.0;
animation.autoreverses = YES;
animation.repeatCount = INFINITY;
animation.duration = 5;
[node addAnimation:animation forKey:nil];
```

A morpher and its target geometries may be loaded from a scene file or created programmatically. The base geometry and all target geometries must be topologically identical—that is, they must contain the same number and structural arrangement of vertices.

## Topics

### Specifying Morph Targets

var targets: [SCNGeometry]

The array of target geometries to morph between.

### Blending between Morph Targets

func weight(forTargetAt: Int) -> CGFloat

Returns the weight value for the specified target index.

func setWeight(CGFloat, forTargetAt: Int)

Specifies a weight value at a specified target index.

### Changing Interpolation Mode

var calculationMode: SCNMorpherCalculationMode

The interpolation formula for blending between target geometries.

### Constants

enum SCNMorpherCalculationMode

The interpolation formulas for blending between target geometries.

### Instance Properties

var unifiesNormals: Bool

var weights: [NSNumber]

### Instance Methods

func setWeight(CGFloat, forTargetNamed: String)

func weight(forTargetNamed: String) -> CGFloat

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- SCNAnimatable

## See Also

### Animation and Constraints

Animation

Create declarative animations that move elements of a scene in predetermined ways, or manage animations imported with external authoring tools.

Constraints

Automatically adjust the position or orientation of a node based on specified rules.

class SCNSkinner

An object that manages the relationship between skeletal animations and the nodes and geometries they animate.

