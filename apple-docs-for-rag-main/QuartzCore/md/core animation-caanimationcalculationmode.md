

- Core Animation
-  CAAnimationCalculationMode 

Structure

# CAAnimationCalculationMode

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CAAnimationCalculationMode
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let cubic: CAAnimationCalculationMode

Smooth spline calculation between keyframe values.

static let cubicPaced: CAAnimationCalculationMode

Cubic keyframe values are interpolated to produce an even pace throughout the animation.

static let discrete: CAAnimationCalculationMode

Each keyframe value is used in turn, no interpolated values are calculated.

static let linear: CAAnimationCalculationMode

Simple linear calculation between keyframe values.

static let paced: CAAnimationCalculationMode

Linear keyframe values are interpolated to produce an even pace throughout the animation.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

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

struct CAShapeLayerLineJoin

