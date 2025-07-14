

- Swift Charts
- NumberBins
-  init(range:desiredCount:minimumStride:) 

Initializer

# init(range:desiredCount:minimumStride:)

Automatically determine the bins from a range of data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    range: ClosedRange,
    desiredCount: Int = 10,
    minimumStride: Value = 0
) where Value : BinaryFloatingPoint
```

## Parameters 

`range`  

The range the bins should cover.

`desiredCount`  

The desired number of bins for the given data. If `nil`, infer the number automatically from data.

`minimumStride`  

The minimum allowed bin size.

## Return Value

The inferred bins.

