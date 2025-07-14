

- Swift Charts
-  ChartProxy 

Structure

# ChartProxy

A proxy that you use to access the scales and plot area of a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ChartProxy
```

## Overview

You get a chart proxy from the chartOverlay(alignment:content:) and chartBackground(alignment:content:) modifiers. You can use the chart proxy to convert data values to screen coordinates or vice-versa.

Below is an example where we convert the screen coordinates from a drag gesture to data values.

```
Chart(data) {
    LineMark(
        x: .value("date", $0.date),
        y: .value("price", $0.price)
    )
}
.chartOverlay { proxy in
    GeometryReader { geometry in
        Rectangle().fill(.clear).contentShape(Rectangle())
            .gesture(
                DragGesture()
                    .onChanged { value in
                        // Convert the gesture location to the coordinate space of the plot area.
                        let origin = geometry[proxy.plotAreaFrame].origin
                        let location = CGPoint(
                            x: value.location.x - origin.x,
                            y: value.location.y - origin.y
                        )
                        // Get the x (date) and y (price) value from the location.
                        let (date, price) = proxy.value(at: location, as: (Date, Double).self)
                        print("Location: \(date), \(price)")
                    }
            )
    }
}
```

## Topics

### Instance Properties

var plotAreaFrame: Anchor&lt;CGRect>

An anchor to the frame of the chart’s plot.

var plotAreaSize: CGSize

The size of the plot in the chart.

var plotContainerFrame: Anchor&lt;CGRect>?

An anchor to the frame of the chart’s plot container, or `nil` if there is no chart in the context of the chart proxy.

var plotFrame: Anchor&lt;CGRect>?

An anchor to the frame of the chart’s plot, or `nil` if there is no chart in the context of the chart proxy.

var plotSize: CGSize

The size of the plot in the chart.

### Instance Methods

func angle(at: CGPoint) -> Angle

Returns the angle relative to the plot area center, where the 12 o’clock position is interpreted as zero degrees, increasing clockwise.

func foregroundStyle&lt;P>(for: P) -> AnyShapeStyle?

Returns the foreground style for the given data value. Returns `nil` if the foreground style scale is unavailable, or the value is invalid.

func foregroundStyleDomain&lt;P>(dataType: P.Type) -> [P]

func lineStyle&lt;P>(for: P) -> StrokeStyle?

Returns the line style for the given data value. Returns `nil` if the line style scale is unavailable, or the value is invalid.

func lineStyleDomain&lt;P>(dataType: P.Type) -> [P]

func position&lt;X, Y>(for: (x: X, y: Y)) -> CGPoint?

Returns the x and y positions as a `CGPoint` for the given data values, or `nil` if either the X or the y scale is unavailable or if any data value is invalid. The returned position is relative to the plot.

func position&lt;P>(forX: P) -> CGFloat?

Returns the x position for the given data value, or `nil` if the x scale is unavailable or if the data value is invalid. The returned position is relative to the plot.

func position&lt;P>(forY: P) -> CGFloat?

Returns the y position for the given data value, or `nil` if the y scale is unavailable or if the data value is invalid. The returned position is relative to the plot.

func positionRange&lt;X, Y>(for: (x: X, y: Y)) -> CGRect?

Returns the range of x and y positions for the given pair of data values, or `nil` if the y scale is unavailable or if the value is invalid.

func positionRange&lt;P>(forX: P) -> ClosedRange&lt;CGFloat>?

Returns the range of x position for the given data value, or `nil` if the x scale is unavailable or if the value is invalid. The returned position range is relative to the plot.

func positionRange&lt;P>(forY: P) -> ClosedRange&lt;CGFloat>?

Returns the range of y position for the given data value, or `nil` if the x scale is unavailable or if the value is invalid. The returned position range is relative to the plot.

func selectAngleValue(at: Angle)

func selectXRange(from: CGFloat, to: CGFloat)

func selectXValue(at: CGFloat)

func selectYRange(from: CGFloat, to: CGFloat)

func selectYValue(at: CGFloat)

func symbol&lt;P>(for: P) -> AnyChartSymbolShape?

Returns the symbol for the given data value. Returns `nil` if the symbol scale is unavailable, or the value is invalid.

func symbolDomain&lt;P>(dataType: P.Type) -> [P]

func symbolSize&lt;P>(for: P) -> CGFloat?

Returns the symbol size for the given data value. Returns `nil` if the symbol size scale is unavailable, or the value is invalid.

func symbolSizeDomain&lt;P>(dataType: P.Type) -> [P]

func value&lt;X, Y>(at: CGPoint, as: (X, Y).Type) -> (X, Y)?

Returns the data values at the given position, or `nil` if the position does not correspond to a valid Y value.

func value&lt;P>(atAngle: Angle, as: P.Type) -> P?

Returns the data value at the given angle, or `nil` if the angle does not correspond to a valid data value.

func value&lt;P>(atX: CGFloat, as: P.Type) -> P?

Returns the data value at the given x position, or `nil` if the position does not correspond to a valid X value.

func value&lt;P>(atY: CGFloat, as: P.Type) -> P?

Returns the data value at the given y position, or `nil` if the position does not correspond to a valid Y value.

func xDomain&lt;P>(dataType: P.Type) -> [P]

func yDomain&lt;P>(dataType: P.Type) -> [P]

## See Also

### Chart management

struct ChartPlotContent

A view that represents a chart’s plot area.

