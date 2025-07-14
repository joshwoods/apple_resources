

- Swift Charts
-  ScaleDomain 

Protocol

# ScaleDomain

A type that you can use to configure the domain of a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ScaleDomain
```

## Topics

### Type Properties

static var automatic: AutomaticScaleDomain

Creates a scale domain configuration that infers the scale domain from data.

### Type Methods

static func automatic(includesZero: Bool?, reversed: Bool?) -> AutomaticScaleDomain

Creates a scale domain configuration that infers the scale domain from data.

static func automatic&lt;DataValue>(includesZero: Bool?, reversed: Bool?, dataType: DataValue.Type, modifyInferredDomain: (inout [DataValue]) -> Void) -> AutomaticScaleDomain

Creates a scale domain configuration that infers the scale domain from data.

## Relationships

### Conforming Types

- AutomaticScaleDomain

## See Also

### Scales

protocol ScaleRange

A type that you can use to configure the range of a chart.

protocol PositionScaleRange

A type that configures the x-axis and y-axis values.

struct PlotDimensionScaleRange

A range that represents the plot area’s width or height.

struct AutomaticScaleDomain

A domain that the chart infers from its data.

struct ScaleType

The ways you can scale the domain or range of a plot.

