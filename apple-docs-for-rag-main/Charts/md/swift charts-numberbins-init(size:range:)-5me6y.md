

- Swift Charts
- NumberBins
-  init(size:range:) 

Initializer

# init(size:range:)

Creates uniform bins covering the given range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    size: Value,
    range: ClosedRange
) where Value : BinaryInteger
```

## Parameters 

`size`  

The size of the bins.

`range`  

The range of the data the bins cover.

## Return Value

The bins.

