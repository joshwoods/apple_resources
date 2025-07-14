

- Swift Charts
- DateBins
-  init(unit:by:range:calendar:) 

Initializer

# init(unit:by:range:calendar:)

Creates uniform bins covering the given range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    unit: Calendar.Component,
    by stride: Int = 1,
    range: ClosedRange,
    calendar: Calendar = .autoupdatingCurrent
)
```

## Parameters 

`unit`  

The size of the bins.

`stride`  

The number of components for each bin.

`range`  

The range of the data the bins cover.

`calendar`  

The calendar to use.

## Return Value

The bins.

