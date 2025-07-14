

- RealityKit
-  BindableData 

Protocol

# BindableData

An opaque base protocol for bindable data objects.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol BindableData
```

## Overview

The templated bindable-value object, BindableValue ``, determines that the value you choose for type `T` adopts this protocol. The types that the framework accepts are: Transform, Float, Double, SIMD2, SIMD3, SIMD4, simd_quatf, Bool, Int, and String.

## Relationships

### Conforming Types

- Transform

## See Also

### Compliance-related protocols

protocol AnimatableData

A functionality specification that animatable data types adopt.

