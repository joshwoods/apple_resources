

- RealityKit
-  AnimatableData 

Protocol

# AnimatableData

A functionality specification that animatable data types adopt.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol AnimatableData
```

## Overview

The templated animation objects, for example BlendTreeAnimation ``, determine that the type you specify for `Value` adopts this protocol. The types that the framework accepts are: JointTransforms, Transform, Float, Double, SIMD2, SIMD3, SIMD4, and simd_quatf.

## Relationships

### Conforming Types

- BlendShapeWeights
- JointTransforms
- Transform

## See Also

### Compliance-related protocols

protocol BindableData

An opaque base protocol for bindable data objects.

