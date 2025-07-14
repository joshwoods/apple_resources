

- Swift Charts
- AreaPlot
-  init(x:yStart:yEnd:domain:function:) 

Initializer

# init(x:yStart:yEnd:domain:function:)

Creates a mark that fills the area between two functions (yStart, yEnd) = f(x).

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    x: S1,
    yStart: S2,
    yEnd: S3,
    domain: ClosedRange? = nil,
    function: @escaping (Double) -> (yStart: Double, yEnd: Double)
) where S1 : StringProtocol, S2 : StringProtocol, S3 : StringProtocol
```

Available when `Content` is `FunctionAreaPlotContent`.

## Discussion

Parameters:

- x: The localized string key for the x label.

- yStart: The localized string key for the start label.

- yEnd: The localized string key for the end label.

- domain: The domain of x. If set to `nil`, the domain of the chart’s x scale will be used.

- function: The function to graph. Returns a tuple of (yStart: yStart, yEnd: yEnd).

Note

For x values where the function is undefined or is infinity, the function is expected to return `Double.nan` or `Double.infinity` respectively.

