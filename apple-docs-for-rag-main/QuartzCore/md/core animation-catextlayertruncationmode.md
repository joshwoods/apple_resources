

- Core Animation
-  CATextLayerTruncationMode 

Structure

# CATextLayerTruncationMode

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CATextLayerTruncationMode
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let end: CATextLayerTruncationMode

Each line is displayed so that the beginning fits in the container and the missing text is indicated by some kind of ellipsis glyph.

static let middle: CATextLayerTruncationMode

Each line is displayed so that the beginning and end fit in the container and the missing text is indicated by some kind of ellipsis glyph in the middle.

static let none: CATextLayerTruncationMode

Each line is displayed so that the text is either wrapped or clipped.

static let start: CATextLayerTruncationMode

Each line is displayed so that the end fits in the container and the missing text is indicated by some kind of ellipsis glyph.

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

