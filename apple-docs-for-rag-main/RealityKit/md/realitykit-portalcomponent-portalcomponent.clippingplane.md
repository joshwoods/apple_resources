

- RealityKit
- PortalComponent
-  PortalComponent.ClippingPlane 

Structure

# PortalComponent.ClippingPlane

A representation of a portal as an infinite plane.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ClippingPlane
```

## Overview

Use this type with init(target:clippingPlane:) to initialize a portal component with the clipping feature in an enabled state.

## Topics

### Initializers

init(position: SIMD3&lt;Float>, normal: SIMD3&lt;Float>)

Creates a clipping plane at a position and normal direction.

### Instance Properties

var normal: SIMD3&lt;Float>

The normal of the clipping plane.

var position: SIMD3&lt;Float>

The position of the clipping plane.

