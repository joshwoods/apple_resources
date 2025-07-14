

- SwiftUI
- View
-  chartOverlay(alignment:content:) 

Instance Method

# chartOverlay(alignment:content:)

Adds an overlay to a view that contains a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func chartOverlay(
    alignment: Alignment = .center,
    @ViewBuilder content: @escaping (ChartProxy) -> V
) -> some View where V : View
```

## Parameters 

`alignment`  

The alignment of the content.

`content`  

The content of the overlay.

## Discussion

You can use this modifier to define an overlay view as a function of the chart in the view. You can access the chart with the `ChartProxy` object passed into the closure.

Below is an example where we define an overlay view that handles drag gestures and use the proxy to convert the gesture coordinates to data values in the chart.

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

Note

If `self` contains more than one chart, the chart proxy will refer to the first chart.

