

- Core Animation
-  CATransitionType 

Structure

# CATransitionType

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CATransitionType
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let fade: CATransitionType

The layer’s content fades as it becomes visible or hidden.

static let moveIn: CATransitionType

The layer’s content slides into place over any existing content.

static let push: CATransitionType

The layer’s content pushes any existing content as it slides into place.

static let reveal: CATransitionType

The layer’s content is revealed gradually in the direction specified by the transition subtype.

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

