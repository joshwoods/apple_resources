

- Core Animation
-  CAMediaTimingFunctionName 

Structure

# CAMediaTimingFunctionName

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CAMediaTimingFunctionName
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let `default`: CAMediaTimingFunctionName

The system default timing function. Use this function to ensure that the timing of your animations matches that of most system animations.

static let easeIn: CAMediaTimingFunctionName

Ease-in pacing, which causes an animation to begin slowly and then speed up as it progresses.

static let easeInEaseOut: CAMediaTimingFunctionName

Ease-in-ease-out pacing, which causes an animation to begin slowly, accelerate through the middle of its duration, and then slow again before completing.

static let easeOut: CAMediaTimingFunctionName

Ease-out pacing, which causes an animation to begin quickly and then slow as it progresses.

static let linear: CAMediaTimingFunctionName

Linear pacing, which causes an animation to occur evenly over its duration.

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

struct CAScrollLayerScrollMode

struct CAShapeLayerFillRule

struct CAShapeLayerLineCap

struct CAShapeLayerLineJoin

