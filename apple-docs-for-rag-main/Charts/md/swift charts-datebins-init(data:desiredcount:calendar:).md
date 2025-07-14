

- Swift Charts
- DateBins
-  init(data:desiredCount:calendar:) 

Initializer

# init(data:desiredCount:calendar:)

Automatically determine the bins from data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    data: [Date],
    desiredCount: Int? = nil,
    calendar: Calendar = .autoupdatingCurrent
)
```

## Parameters 

`data`  

The given data values.

`desiredCount`  

The desired number of bins for the given data. If `nil`, infer the number of bins automatically from data using Scott’s normal reference rule capped at 200.

## Return Value

The inferred bins.

