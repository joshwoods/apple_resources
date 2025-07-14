

- RealityKit
- IKRig
- IKRig.Joint
-  IKRig.Joint.LimitsDefinition 

Structure

# IKRig.Joint.LimitsDefinition

A definition of joint rotation limits.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct LimitsDefinition
```

## Overview

Limit angles are defined as relative to the rest pose.

Important

The minimum angles need to be less than the maximum angles.

## Topics

### Initializers

init(weight: Float, boneAxis: IKRig.Joint.LimitsDefinition.Axis, minimumAngles: SIMD3&lt;Float>, maximumAngles: SIMD3&lt;Float>)

Creates a joint limits definition.

### Instance Properties

var boneAxis: IKRig.Joint.LimitsDefinition.Axis

The axis around which the bone twists.

var maximumAngles: SIMD3&lt;Float>

The positive delta from the rest pose per-axis in radians.

var minimumAngles: SIMD3&lt;Float>

The negative delta from the rest pose per-axis in radians.

var weight: Float

The weight of the joint rotation limit demand.

### Enumerations

enum Axis

