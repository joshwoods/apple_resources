

- Core Animation
-  CAValueFunctionName 

Structure

# CAValueFunctionName

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
struct CAValueFunctionName
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let rotateX: CAValueFunctionName

A value function that rotates by the input value, in radians, around the x-axis. This value function expects a single input value.

static let rotateY: CAValueFunctionName

A value function that rotates by the input value, in radians, around the y-axis. This value function expects a single input value.

static let rotateZ: CAValueFunctionName

A value function that rotates by the input value, in radians, around the z-axis. This value function expects a single input value.

static let scale: CAValueFunctionName

A value function scales by the input value along all three axis. Animations using this value transform function must provide animation values in an `NSArray` of three `NSNumber` instances that specify the (x, y, z) scale values.

static let scaleX: CAValueFunctionName

A value function scales by the input value along the x-axis. Animations referencing this value transform function must provide a single animation value.

static let scaleY: CAValueFunctionName

A value function scales by the input value along the y-axis. Animations referencing this value function must provide a single animation value.

static let scaleZ: CAValueFunctionName

A value function that scales by the input value along the z-axis. Animations referencing this value function must provide a single animation value.

static let translate: CAValueFunctionName

A value function that translates by the input values along all three axis. Animations using this value transform function must provide animation values in an `NSArray` of three `NSNumber` instances that specify the (x, y, z) translate values.

static let translateX: CAValueFunctionName

A value function translates by the input value along the x-axis. Animations referencing this value function must provide a single input value.

static let translateY: CAValueFunctionName

A value function translates by the input value along the y-axis. Animations referencing this value function must provide a single input value.

static let translateZ: CAValueFunctionName

A value function translates by the input value along the z-axis. Animations referencing this value function must provide a single input value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

struct CAAnimationCalculationMode

struct CAAnimationRotationMode

struct CAEmitterLayerEmitterMode

struct CAEmitterLayerEmitterShape

struct CAEmitterLayerRenderMode

struct CAGradientLayerType

struct CALayerContentsFilter

struct CALayerContentsFormat

struct CALayerContentsGravity

struct CALayerCornerCurve

struct CAMediaTimingFillMode

struct CAMediaTimingFunctionName

struct CAScrollLayerScrollMode

struct CAShapeLayerFillRule

struct CAShapeLayerLineCap

