

- TabularData
- NumericSummary
-  init(someCount:noneCount:mean:standardDeviation:min:max:median:firstQuartile:thirdQuartile:) 

Initializer

# init(someCount:noneCount:mean:standardDeviation:min:max:median:firstQuartile:thirdQuartile:)

Creates an empty numeric summary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    someCount: Int,
    noneCount: Int,
    mean: Element,
    standardDeviation: Element,
    min: Element,
    max: Element,
    median: Element,
    firstQuartile: Element,
    thirdQuartile: Element
)
```

## Parameters 

`someCount`  

The number of elements in column, excluding missing elements.

`noneCount`  

The number of missing elements in the column.

`mean`  

The arithmetic mean of a column’s values, excluding missing elements.

`standardDeviation`  

The standard deviation of a column’s values, excluding missing elements.

`min`  

The smallest value, excluding missing elements.

`max`  

The largest value, excluding missing elements.

`median`  

The midpoint value that bisects the values of the non-missing elements.

`firstQuartile`  

The value that’s above 25% of the values non-missing elements’ values.

`thirdQuartile`  

The value that’s above 75% of the non-missing elements’ values.

## See Also

### Creating a Summary

init()

Creates an empty numeric summary with default values.

