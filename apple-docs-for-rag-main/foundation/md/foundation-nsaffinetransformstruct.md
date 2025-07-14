

- Foundation
-  NSAffineTransformStruct 

Structure

# NSAffineTransformStruct

A structure that defines the three-by-three matrix that performs an affine transform between two coordinate systems.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct NSAffineTransformStruct
```

## Overview

For more details, see Cocoa Drawing Guide.

## Topics

### Initializers

init()

Initializes a zero-filled transformation matrix.

init(m11: Double, m12: Double, m21: Double, m22: Double, tX: Double, tY: Double)

### Instance Properties

var m11: Double

An element of the transform matrix that contributes scaling, rotation, and shear.

var m12: Double

An element of the transform matrix that contributes scaling, rotation, and shear.

var m21: Double

An element of the transform matrix that contributes scaling, rotation, and shear.

var m22: Double

An element of the transform matrix that contributes scaling, rotation, and shear.

var tX: Double

An element of the transform matrix that contributes translation.

var tY: Double

An element of the transform matrix that contributes translation.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing the Transformation Matrix

var transformStruct: NSAffineTransformStruct

The matrix coefficients stored as the transformation matrix.

