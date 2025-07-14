

- SwiftUI
- View
-  chartXScale(type:) 

Instance Method

# chartXScale(type:)

Configures the x scale for charts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartXScale(type: ScaleType? = nil) -> some View
```

## Parameters 

`type`  

The scale type.

## See Also

### Axis scales

func chartXScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartXScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the x scale for charts.

func chartYScale&lt;Domain, Range>(domain: Domain, range: Range, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale&lt;Domain>(domain: Domain, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale&lt;Range>(range: Range, type: ScaleType?) -> some View

Configures the y scale for charts.

func chartYScale(type: ScaleType?) -> some View

Configures the y scale for charts.

