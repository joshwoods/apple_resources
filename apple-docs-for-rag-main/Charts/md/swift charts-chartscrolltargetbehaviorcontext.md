

- Swift Charts
-  ChartScrollTargetBehaviorContext 

Structure

# ChartScrollTargetBehaviorContext

Contextual information that you can use to determine how to best adjust how charts scroll.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@dynamicMemberLookup
struct ChartScrollTargetBehaviorContext
```

## Topics

### Instance Properties

var chartProxy: ChartProxy

The chart proxy that you use to access the scales and plot area of the chart.

### Subscripts

subscript&lt;T>(dynamicMember _: KeyPath&lt;ScrollTargetBehaviorContext, T>) -> T

## See Also

### Scrolling

protocol ChartScrollTargetBehavior

A type that configures the scroll behavior of charts.

