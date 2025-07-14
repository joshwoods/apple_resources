

- Swift Charts
-  MarkStackingMethod 

Structure

# MarkStackingMethod

The ways in which you can stack marks in a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct MarkStackingMethod
```

## Topics

### Type Properties

static var center: MarkStackingMethod

Stack marks using a center offset.

static var normalized: MarkStackingMethod

Create normalized stacked bar and area charts.

static var standard: MarkStackingMethod

Stack marks starting at zero.

static var unstacked: MarkStackingMethod

Don’t stack marks.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Mark configuration

struct MarkDimension

An individual dimension representing a mark’s width or height.

struct InterpolationMethod

The ways in which line or area marks interpolate their data.

struct BasicChartSymbolShape

A basic chart symbol shape.

protocol ChartSymbolShape

A type that can act as a shape for the marks that you add to a chart.

struct AnyChartSymbolShape

A type-erased plotting shape.

