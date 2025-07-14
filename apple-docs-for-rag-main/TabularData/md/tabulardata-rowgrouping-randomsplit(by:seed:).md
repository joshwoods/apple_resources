

- TabularData
- RowGrouping
-  randomSplit(by:seed:) 

Instance Method

# randomSplit(by:seed:)

Generates two row groupings by randomly splitting the original with a proportion and a seed number.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func randomSplit(
    by proportion: Double,
    seed: Int? = nil
) -> (RowGrouping, RowGrouping)
```

Available when `GroupingKey` conforms to `Hashable`.

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`seed`  

A seed number for a random-number generator.

## Return Value

A tuple of two row groupings.

## See Also

### Splitting a Row Grouping

func randomSplit(by: Double) -> (Self, Self)

Generates two row groupings by randomly splitting the original with a proportion.

