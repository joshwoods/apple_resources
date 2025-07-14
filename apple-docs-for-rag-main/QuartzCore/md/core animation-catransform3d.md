

- Core Animation
-  CATransform3D 

Structure

# CATransform3D

The standard transform matrix used throughout Core Animation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CATransform3D
```

## Overview

The transform matrix is used to rotate, scale, translate, skew, and project the layer content. Functions are provided for creating, concatenating, and modifying CATransform3D data.

## Topics

### Initializers

init()

init(m11: CGFloat, m12: CGFloat, m13: CGFloat, m14: CGFloat, m21: CGFloat, m22: CGFloat, m23: CGFloat, m24: CGFloat, m31: CGFloat, m32: CGFloat, m33: CGFloat, m34: CGFloat, m41: CGFloat, m42: CGFloat, m43: CGFloat, m44: CGFloat)

init(float4x4)

init(double4x4)

### Instance Properties

var m11: CGFloat

The entry at position 1,1 in the matrix.

var m12: CGFloat

The entry at position 1,2 in the matrix.

var m13: CGFloat

The entry at position 1,3 in the matrix.

var m14: CGFloat

The entry at position 1,4 in the matrix.

var m21: CGFloat

The entry at position 2,1 in the matrix.

var m22: CGFloat

The entry at position 2,2 in the matrix.

var m23: CGFloat

The entry at position 2,3 in the matrix.

var m24: CGFloat

The entry at position 2,4 in the matrix.

var m31: CGFloat

The entry at position 3,1 in the matrix.

var m32: CGFloat

The entry at position 3,2 in the matrix.

var m33: CGFloat

The entry at position 3,3 in the matrix.

var m34: CGFloat

The entry at position 3,4 in the matrix.

var m41: CGFloat

The entry at position 4,1 in the matrix.

var m42: CGFloat

The entry at position 4,2 in the matrix.

var m43: CGFloat

The entry at position 4,3 in the matrix.

var m44: CGFloat

The entry at position 4,4 in the matrix.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

## See Also

### Constants

struct CAAutoresizingMask

These constants are used by the autoresizingMask property.

Action Identifiers

These constants are the predefined action identifiers used by action(forKey:), add(_:forKey:), defaultAction(forKey:), removeAnimation(forKey:), Layer Filters, and the CAAction protocol method run(forKey:object:arguments:).

struct CAEdgeAntialiasingMask

This mask is used by the edgeAntialiasingMask property.

Identity Transform

Defines the identity transform matrix used by Core Animation.

Scaling Filters

These constants specify the scaling filters used by magnificationFilter and minificationFilter.

