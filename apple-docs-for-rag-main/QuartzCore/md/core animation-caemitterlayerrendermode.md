

- Core Animation
-  CAEmitterLayerRenderMode 

Structure

# CAEmitterLayerRenderMode

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
struct CAEmitterLayerRenderMode
```

## Topics

### Initializers

init(rawValue: String)

### Type Properties

static let additive: CAEmitterLayerRenderMode

The particles are rendered using source-additive compositing.

static let backToFront: CAEmitterLayerRenderMode

Particles are rendered from back to front, sorted by z-position. This mode uses source-over compositing.

static let oldestFirst: CAEmitterLayerRenderMode

Particles are rendered oldest first. This mode uses source-over compositing.

static let oldestLast: CAEmitterLayerRenderMode

Particles are rendered oldest last. This mode uses source-over compositing.

static let unordered: CAEmitterLayerRenderMode

Particles are rendered unordered. This mode uses source-over compositing.

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

