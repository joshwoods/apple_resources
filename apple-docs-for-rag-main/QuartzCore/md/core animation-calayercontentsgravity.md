

- Core Animation
-  CALayerContentsGravity 

Structure

# CALayerContentsGravity

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
struct CALayerContentsGravity
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let bottom: CALayerContentsGravity

The content is horizontally centered at the bottom-edge of the bounds rectangle.

static let bottomLeft: CALayerContentsGravity

The content is positioned in the bottom-left corner of the bounds rectangle.

static let bottomRight: CALayerContentsGravity

The content is positioned in the bottom-right corner of the bounds rectangle.

static let center: CALayerContentsGravity

The content is horizontally and vertically centered in the bounds rectangle.

static let left: CALayerContentsGravity

The content is vertically centered at the left-edge of the bounds rectangle.

static let resize: CALayerContentsGravity

The content is resized to fit the entire bounds rectangle.

static let resizeAspect: CALayerContentsGravity

The content is resized to fit the bounds rectangle, preserving the aspect of the content. If the content does not completely fill the bounds rectangle, the content is centered in the partial axis.

static let resizeAspectFill: CALayerContentsGravity

The content is resized to completely fill the bounds rectangle, while still preserving the aspect of the content. The content is centered in the axis it exceeds.

static let right: CALayerContentsGravity

The content is vertically centered at the right-edge of the bounds rectangle.

static let top: CALayerContentsGravity

The content is horizontally centered at the top-edge of the bounds rectangle.

static let topLeft: CALayerContentsGravity

The content is positioned in the top-left corner of the bounds rectangle.

static let topRight: CALayerContentsGravity

The content is positioned in the top-right corner of the bounds rectangle.

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

struct CALayerCornerCurve

struct CAMediaTimingFillMode

struct CAMediaTimingFunctionName

struct CAScrollLayerScrollMode

struct CAShapeLayerFillRule

struct CAShapeLayerLineCap

struct CAShapeLayerLineJoin

