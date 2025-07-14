

- Swift
- AsyncStream
-  min(by:) 

Instance Method

# min(by:)

Returns the minimum element in the asynchronous sequence, using the given predicate as the comparison between elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@warn_unqualified_access
func min(by areInIncreasingOrder: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?
```

## Parameters 

`areInIncreasingOrder`  

A predicate that returns `true` if its first argument should be ordered before its second argument; otherwise, `false`.

## Return Value

The sequence’s minimum element, according to `areInIncreasingOrder`. If the sequence has no elements, returns `nil`.

## Discussion

Use this method when the asynchronous sequence’s values don’t conform to `Comparable`, or when you want to apply a custom ordering to the sequence.

The predicate must be a *strict weak ordering* over the elements. That is, for any elements `a`, `b`, and `c`, the following conditions must hold:

- `areInIncreasingOrder(a, a)` is always `false`. (Irreflexivity)

- If `areInIncreasingOrder(a, b)` and `areInIncreasingOrder(b, c)` are both `true`, then `areInIncreasingOrder(a, c)` is also `true`. (Transitive comparability)

- Two elements are *incomparable* if neither is ordered before the other according to the predicate. If `a` and `b` are incomparable, and `b` and `c` are incomparable, then `a` and `c` are also incomparable. (Transitive incomparability)

The following example uses an enumeration of playing cards ranks, `Rank`, which ranges from `ace` (low) to `king` (high). An asynchronous sequence called `RankCounter` produces all elements of the array. The predicate provided to the `min(by:)` method sorts ranks based on their `rawValue`:

```
enum Rank: Int {
    case ace = 1, two, three, four, five, six, seven, eight, nine, ten, jack, queen, king
}

let min = await RankCounter()
    .min { $0.rawValue 

## See Also

### Finding Elements

func contains(Self.Element) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains the given element.

func contains(where: (Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func first(where: (Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func min() async rethrows -> Self.Element?

Returns the minimum element in an asynchronous sequence of comparable elements.

func max() async rethrows -> Self.Element?

Returns the maximum element in an asynchronous sequence of comparable elements.

func max(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the maximum element in the asynchronous sequence, using the given predicate as the comparison between elements.

