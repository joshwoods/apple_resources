

- Swift Charts
-  InterpolationMethod 

Structure

# InterpolationMethod

The ways in which line or area marks interpolate their data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct InterpolationMethod
```

## Topics

### Type Properties

static var cardinal: InterpolationMethod

Interpolate data points with cardinal spline.

static var catmullRom: InterpolationMethod

Interpolate data points with Catmull-Rom spline.

static var linear: InterpolationMethod

Interpolate data points linearly.

static var monotone: InterpolationMethod

Interpolate data points with a cubic spline that preserves monotonicity of the data.

static var stepCenter: InterpolationMethod

Interpolate data points with a step, or piece-wise constant function, where the data point is at the center of the step.

static var stepEnd: InterpolationMethod

Interpolate data points with a step, or piece-wise constant function, where the data point is at the end of the step.

static var stepStart: InterpolationMethod

Interpolate data points with a step, or piece-wise constant function, where the data point is at the start of the step.

### Type Methods

static func cardinal(tension: CGFloat) -> InterpolationMethod

Interpolate data points with cardinal spline, using the given tension parameter.

static func catmullRom(alpha: CGFloat) -> InterpolationMethod

Interpolate data points with Catmull-Rom spline, using the given alpha parameter.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
- Sendable

## See Also

### Mark configuration

struct MarkStackingMethod

The ways in which you can stack marks in a chart.

struct MarkDimension

An individual dimension representing a mark’s width or height.

struct BasicChartSymbolShape

A basic chart symbol shape.

protocol ChartSymbolShape

A type that can act as a shape for the marks that you add to a chart.

struct AnyChartSymbolShape

A type-erased plotting shape.

