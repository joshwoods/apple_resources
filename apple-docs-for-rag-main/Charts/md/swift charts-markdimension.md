

- Swift Charts
-  MarkDimension 

Structure

# MarkDimension

An individual dimension representing a mark’s width or height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct MarkDimension
```

## Topics

### Supporting types

struct MarkDimensions

### Initializers

init(floatLiteral: Double)

Creates a constant width or height from a floating point value.

init(integerLiteral: Int)

Creates a constant width or height from an integer.

### Type Properties

static var automatic: MarkDimension

A dimension that determines its value automatically.

### Type Methods

static func fixed(CGFloat) -> MarkDimension

A constant dimension.

static func inset(CGFloat) -> MarkDimension

A dimension that’s the step size minus the specified inset value on each side.

static func ratio(CGFloat) -> MarkDimension

A dimension that’s proportional to the scale step size, using the specified ratio.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Sendable

## See Also

### Mark configuration

struct MarkStackingMethod

The ways in which you can stack marks in a chart.

struct InterpolationMethod

The ways in which line or area marks interpolate their data.

struct BasicChartSymbolShape

A basic chart symbol shape.

protocol ChartSymbolShape

A type that can act as a shape for the marks that you add to a chart.

struct AnyChartSymbolShape

A type-erased plotting shape.

