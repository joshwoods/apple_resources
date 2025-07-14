

- Swift Charts
- ChartProxy
-  plotContainerFrame 

Instance Property

# plotContainerFrame

An anchor to the frame of the chart’s plot container, or `nil` if there is no chart in the context of the chart proxy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var plotContainerFrame: Anchor? { get }
```

## Discussion

The plot is the area between the x and y axes, not including the axes themselves. If the chart is scrollable, the plot container frame only includes the visible portion of the plot. Otherwise, it is the same as plotFrame.

You can convert the anchor to a frame using a `GeometryProxy`. Below is an example adding a border to the plot container:

```
Chart { ... }
.chartOverlay { chartProxy in
    GeometryReader { geometryProxy in
        // Get the plot container's frame in the GeometryReader's coordinate space.
        // This frame stays the same when the chart scrolls.
        // In this example, we add a border to the plot container by stroking the frame.
        if let plotContainerFrame = chartProxy.plotContainerFrame {
            Path(geometryProxy[plotContainerFrame])
                .stroke(.black, lineWidth: 1)
                .allowsHitTesting(false)
        }
    }
}
```

