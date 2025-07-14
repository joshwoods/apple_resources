

- Core Animation
-  CAShapeLayerFillRule 

Structure

# CAShapeLayerFillRule

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
struct CAShapeLayerFillRule
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let evenOdd: CAShapeLayerFillRule

Specifies the even-odd winding rule. Count the total number of path crossings. If the number of crossings is even, the point is outside the path. If the number of crossings is odd, the point is inside the path and the region containing it should be filled.

static let nonZero: CAShapeLayerFillRule

Specifies the non-zero winding rule. Count each left-to-right path as +1 and each right-to-left path as -1. If the sum of all crossings is 0, the point is outside the path. If the sum is nonzero, the point is inside the path and the region containing it is filled.

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

struct CAShapeLayerLineCap

struct CAShapeLayerLineJoin

