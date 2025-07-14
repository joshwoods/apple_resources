

- Core Animation
-  CAMediaTimingFillMode 

Structure

# CAMediaTimingFillMode

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CAMediaTimingFillMode
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let backwards: CAMediaTimingFillMode

The receiver clamps values before zero to zero when the animation is completed.

static let both: CAMediaTimingFillMode

The receiver clamps values at both ends of the object’s time space

static let forwards: CAMediaTimingFillMode

The receiver remains visible in its final state when the animation is completed.

static let removed: CAMediaTimingFillMode

The receiver is removed from the presentation when the animation is completed.

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

struct CAMediaTimingFunctionName

struct CAScrollLayerScrollMode

struct CAShapeLayerFillRule

struct CAShapeLayerLineCap

struct CAShapeLayerLineJoin

