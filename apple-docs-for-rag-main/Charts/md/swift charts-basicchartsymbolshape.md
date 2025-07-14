

- Swift Charts
-  BasicChartSymbolShape 

Structure

# BasicChartSymbolShape

A basic chart symbol shape.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct BasicChartSymbolShape
```

## Topics

### Instance Methods

func strokeBorder(lineWidth: CGFloat) -> some ChartSymbolShape

Creates a stroked symbol shape by inner-stroking the basic symbol shape.

## Relationships

### Conforms To

- Animatable
- ChartSymbolShape
- Sendable
- Shape
- View

## See Also

### Mark configuration

struct MarkStackingMethod

The ways in which you can stack marks in a chart.

struct MarkDimension

An individual dimension representing a mark’s width or height.

struct InterpolationMethod

The ways in which line or area marks interpolate their data.

protocol ChartSymbolShape

A type that can act as a shape for the marks that you add to a chart.

struct AnyChartSymbolShape

A type-erased plotting shape.

