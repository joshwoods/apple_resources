

- SceneKit
-  SCNVector4 

Structure

# SCNVector4

A representation of a four-component vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SCNVector4
```

## Overview

SceneKit uses four-component vectors to represent multiple kinds of data:

- Axis-angle rotation or torque. The `x`, `y`, and `z` fields contain the normalized x-, y-, and z-components of the rotation axis, and the `w` field contains the rotation angle, in radians, or torque magnitude, in newton-meters.

- Color value (or range). The `x`, `y`, `z`, and `w` fields contain the red, green, blue, and alpha components of the color, or the width of the color variation range in each component.

Important

In macOS, the `x`, `y`, `z` and `w` fields in this structure are CGFloat values. In iOS, tvOS, and watchOS, these fields are `float` values.

## Topics

### Components

var x: Float

The first component in the vector.

var y: Float

The second component in the vector.

var z: Float

The third component in the vector.

var w: Float

The fourth component in the vector.

### Creating Vectors

func SCNVector4Make(Float, Float, Float, Float) -> SCNVector4

Returns a new four-component vector created from individual component values.

### Converting Vector Types

func SCNVector4FromGLKVector4(GLKVector4) -> SCNVector4

Returns a four-element SceneKit vector structure corresponding to a GLKit vector structure.

func SCNVector4ToGLKVector4(SCNVector4) -> GLKVector4

Returns a four-element GLKit vector structure corresponding to a SceneKit vector structure.

### Comparing Vectors

func SCNVector4EqualToVector4(SCNVector4, SCNVector4) -> Bool

Returns a Boolean value that indicates whether the corresponding components of two vectors are equal.

### Zero Constant

let SCNVector4Zero: SCNVector4

The four-component vector whose every component is `0.0`.

### Initializers

init()

init(SIMD4&lt;Double>)

init(SIMD4&lt;Float>)

init(Int, Int, Int, Int)

init(Double, Double, Double, Double)

init(CGFloat, CGFloat, CGFloat, CGFloat)

init(Float, Float, Float, Float)

init(x: Float, y: Float, z: Float, w: Float)

init(x: CGFloat, y: CGFloat, z: CGFloat, w: CGFloat)

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Vectors

struct SCNVector3

A representation of a three-component vector.

