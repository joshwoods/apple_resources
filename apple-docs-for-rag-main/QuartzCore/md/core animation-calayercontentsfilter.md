

- Core Animation
-  CALayerContentsFilter 

Structure

# CALayerContentsFilter

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CALayerContentsFilter
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let linear: CALayerContentsFilter

Linear interpolation filter.

static let nearest: CALayerContentsFilter

Nearest neighbor interpolation filter.

static let trilinear: CALayerContentsFilter

Trilinear minification filter. Enables mipmap generation. Some renderers may ignore this, or impose additional restrictions, such as source images requiring power-of-two dimensions.

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

struct CALayerContentsFormat

struct CALayerContentsGravity

struct CALayerCornerCurve

struct CAMediaTimingFillMode

struct CAMediaTimingFunctionName

struct CAScrollLayerScrollMode

struct CAShapeLayerFillRule

struct CAShapeLayerLineCap

struct CAShapeLayerLineJoin

