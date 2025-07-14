

- Foundation
- Data
-  first(where:) 

Instance Method

# first(where:)

Returns the first element of the sequence that satisfies the given predicate.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func first(where predicate: (Self.Element) throws -> Bool) rethrows -> Self.Element?
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns a Boolean value indicating whether the element is a match.

## Return Value

The first element of the sequence that satisfies `predicate`, or `nil` if there is no element that satisfies `predicate`.

## Discussion

The following example uses the `first(where:)` method to find the first negative number in an array of integers:

```
let numbers = [3, 7, 4, -2, 9, -6, 10, 1]
if let firstNegative = numbers.first(where: { $0 

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Finding Bytes

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min() -> Self.Element?

Returns the minimum element in the sequence.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func range(of: Data, options: Data.SearchOptions, in: Range&lt;Data.Index>?) -> Range&lt;Data.Index>?

Finds the range of the specified data as a subsequence of this data, if it exists.

typealias SearchOptions

Options that control a data search operation.

