

- TabularData
- FilledColumn
-  min() 

Instance Method

# min()

Returns the minimum element in the sequence.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@warn_unqualified_access
func min() -> Self.Element?
```

Available when `Element` conforms to `Comparable`.

## Return Value

The sequence’s minimum element. If the sequence has no elements, returns `nil`.

## Discussion

This example finds the smallest value in an array of height measurements.

```
let heights = [67.5, 65.7, 64.3, 61.1, 58.5, 60.3, 64.9]
let lowestHeight = heights.min()
print(lowestHeight)
// Prints "Optional(58.5)"
```

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Finding Elements

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

