

- Swift
- AsyncStream
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the asynchronous sequence contains the given element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func contains(_ search: Self.Element) async rethrows -> Bool
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`search`  

The element to find in the asynchronous sequence.

## Return Value

`true` if the method found the element in the asynchronous sequence; otherwise, `false`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `contains(_:)` method checks to see whether the sequence produces the value `5`:

```
let containsFive = await Counter(howHigh: 10)
    .contains(5)
print(containsFive)
// Prints "true"
```

## See Also

### Finding Elements

func contains(where: (Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func first(where: (Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func min() async rethrows -> Self.Element?

Returns the minimum element in an asynchronous sequence of comparable elements.

func min(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the minimum element in the asynchronous sequence, using the given predicate as the comparison between elements.

func max() async rethrows -> Self.Element?

Returns the maximum element in an asynchronous sequence of comparable elements.

func max(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the maximum element in the asynchronous sequence, using the given predicate as the comparison between elements.

