

- SpriteKit
-  SKTransformNode 

Class

# SKTransformNode

A node that allows its children to rotate in 3D.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

**watchOS**

``` source
class SKTransformNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKTransformNode
```

## Overview

`SKTranformNode` adds the ability to rotate nodes across the x and y axes. When combined with `SKNode`’s zRotation property, nodes added as children to a transform node have the ability to rotate in 3D.

## Topics

### Rotating Child Nodes

var xRotation: CGFloat

var yRotation: CGFloat

func setEulerAngles(vector_float3)

func setQuaternion(simd_quatf)

func setRotationMatrix(matrix_float3x3)

### Reading the Current Rotation

func eulerAngles() -> vector_float3

func quaternion() -> simd_quatf

func rotationMatrix() -> matrix_float3x3

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Nodes that Modify Drawing

class SKEffectNode

A node that renders its children into a separate buffer, optionally applying an effect, before drawing the final result.

class SKCropNode

A node that masks pixels drawn by its children so that only some pixels are seen.

