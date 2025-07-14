

- TabularData
- RowGroupingProtocol
-  randomSplit(by:) 

Instance Method

# randomSplit(by:)

Generates two row groupings by randomly splitting the original with a proportion.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func randomSplit(by proportion: Double) -> (Self, Self)
```

## Return Value

A tuple of two row groupings.

## See Also

### Splitting a Row Grouping

func randomSplit(by: Double, seed: Int?) -> (Self, Self)

Generates two row groupings by randomly splitting the original by a proportion.

**Required**

