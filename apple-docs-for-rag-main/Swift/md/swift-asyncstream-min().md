

- Swift
- AsyncStream
-  min() 

Instance Method

# min()

Returns the minimum element in an asynchronous sequence of comparable elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@warn_unqualified_access
func min() async rethrows -> Self.Element?
```

Available when `Element` conforms to `Comparable`.

## Return Value

The sequence’s minimum element. If the sequence has no elements, returns `nil`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `min()` method returns the minimum value of the sequence.

```
let min = await Counter(howHigh: 10)
    .min()
print(min ?? "none")
// Prints "1"
```

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

func min(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the minimum element in the asynchronous sequence, using the given predicate as the comparison between elements.

func max() async rethrows -> Self.Element?

Returns the maximum element in an asynchronous sequence of comparable elements.

func max(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the maximum element in the asynchronous sequence, using the given predicate as the comparison between elements.

