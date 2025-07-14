

- Swift Charts
-  AreaMark 

Structure

# AreaMark

Chart content that represents data using the area of one or more regions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct AreaMark
```

## Overview

Use `AreaMark` to represent data as filled regions on a chart. To create a simple area mark chart, plot a date or an ordered string property on the x-axis, and a number on the y-axis. For example, suppose you have data that represents the cost of a cheeseburger over time, stored in an array of `Food` structures:

```
```

You can create labeled data in the form of PlottableValue instances for each of the `x` and `y` inputs to an area mark:

```
```

The resulting chart automatically scales and labels the axes based on the data, and fills the area under the data points with a default color:

If you want only the line without filling in the area below the line, use LineMark instead.

### Add detail with a stacked area chart

To represent an additional dimension of information, you can create a stacked area chart. For example, suppose you have another data set that represents the same cost data from the previous example, but which is broken into the component costs for the burger, bun, and cheese:

```
```

You can again create an area mark with the data, but in this case add the foregroundStyle(by:) modifier to create a stacked area chart that divides the information into distinct regions based on the data’s `name` property:

```
```

The chart automatically assigns a different color to each region, and adds a legend that indicates what each color represents based on the names that you provide to the modifier:

### Stack the data in different ways

You can highlight different aspects of the data by stacking it in different ways. For example, the previous chart shows the absolute contributions of each ingredient to the cheeseburger’s total cost. To see the relative contributions instead, you can create a normalized chart by setting the area mark’s `stacking` parameter to normalized:

```
```

Alternatively, you can use center stacking to create a streamgraph, which shifts the area chart’s baseline to the center of the chart’s plotting area:

```
```

### Create a range area chart

You can also use area marks to create a range area chart, where you provide an interval to fill in for each data point. To do this, you provide either a date or ordered string category for the x-axis and a range of values for the y-axis, or vice versa. For example, suppose you record the minimum and maximum temperatures every day in a `Weather` structure:

```
```

If you load a collection of these structures into a `data` array, you can use the date on the x-axis, and each day’s minimum and maximum temperature as the start and end points for the y-axis:

```
```

This creates a filled region that’s shaped by the start and end points on each date:

```
```

## Topics

### Creating an area mark

init&lt;X, Y>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, stacking: MarkStackingMethod)

Creates an area mark using the specified horizontal and vertical positions.

init&lt;X, Y, S>(x: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>, stacking: MarkStackingMethod)

Creates an area mark and associates it with the specified series.

### Creating a range area chart

init&lt;X, Y>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>)

Creates an area mark that plots values with a vertical interval.

init&lt;X, Y, S>(x: PlottableValue&lt;X>, yStart: PlottableValue&lt;Y>, yEnd: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a vertical interval and associates it with the specified series.

init&lt;X, Y>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>)

Creates an area mark that plots values with a horizontal interval.

init&lt;X, Y, S>(xStart: PlottableValue&lt;X>, xEnd: PlottableValue&lt;X>, y: PlottableValue&lt;Y>, series: PlottableValue&lt;S>)

Creates an area mark that plots values with a horizontal interval and associates it with the specified series.

## Relationships

### Conforms To

- ChartContent
- Copyable
- Sendable

## See Also

### Marks

struct LineMark

Chart content that represents data using a sequence of connected line segments.

struct PointMark

Chart content that represents data using points.

struct RectangleMark

Chart content that represents data using rectangles.

struct RuleMark

Chart content that represents data using a single horizontal or vertical rule.

struct BarMark

Chart content that represents data using bars.

struct SectorMark

A sector of a pie or donut chart, which shows how individual categories make up a meaningful total.

