

- SceneKit
-  SCNVector3 

Structure

# SCNVector3

A representation of a three-component vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SCNVector3
```

## Overview

SceneKit uses three-component vectors for a variety of purposes, such as describing node or vertex positions, surface normals, and scale or translation transforms. The different vector components should be interpreted based on the context in which the vector is being used.

Important

In macOS, the `x`, `y`, and `z` fields in this structure are CGFloat values. In iOS, tvOS, and watchOS, these fields are `float` values.

## Topics

### Components

var x: Float

The first component in the vector.

var y: Float

The second component in the vector.

var z: Float

The third component in the vector.

### Creating Vectors

func SCNVector3Make(Float, Float, Float) -> SCNVector3

Returns a new three-component vector created from individual component values.

### Converting Vector Types

func SCNVector3FromGLKVector3(GLKVector3) -> SCNVector3

Returns a three-element SceneKit vector structure corresponding to a GLKit vector structure.

func SCNVector3ToGLKVector3(SCNVector3) -> GLKVector3

Returns a three-element GLKit vector structure corresponding to a SceneKit vector structure.

### Comparing Vectors

func SCNVector3EqualToVector3(SCNVector3, SCNVector3) -> Bool

Returns a Boolean value that indicates whether the corresponding components of two vectors are equal.

### Zero Constant

let SCNVector3Zero: SCNVector3

The three-component vector whose every component is `0.0`.

### Initializers

init()

init(SIMD3&lt;Double>)

init(SIMD3&lt;Float>)

init(Int, Int, Int)

init(CGFloat, CGFloat, CGFloat)

init(Double, Double, Double)

init(Float, Float, Float)

init(x: CGFloat, y: CGFloat, z: CGFloat)

init(x: Float, y: Float, z: Float)

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Vectors

struct SCNVector4

A representation of a four-component vector.

