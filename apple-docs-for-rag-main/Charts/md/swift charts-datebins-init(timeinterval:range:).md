

- Swift Charts
- DateBins
-  init(timeInterval:range:) 

Initializer

# init(timeInterval:range:)

Creates uniform bins covering the given range. The first bin starts at the lower bound of the range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    timeInterval: TimeInterval,
    range: ClosedRange
)
```

## Parameters 

`timeInterval`  

The size of the bins.

`range`  

The range of the data the bins cover.

## Return Value

The bins.

