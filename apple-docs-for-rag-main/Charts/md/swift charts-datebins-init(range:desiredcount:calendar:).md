

- Swift Charts
- DateBins
-  init(range:desiredCount:calendar:) 

Initializer

# init(range:desiredCount:calendar:)

Automatically determine the bins from a range of data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    range: ClosedRange,
    desiredCount: Int = 10,
    calendar: Calendar = .autoupdatingCurrent
)
```

## Parameters 

`range`  

The range the bins should cover.

`desiredCount`  

The desired number of bins for the given data.

## Return Value

The inferred bins.

