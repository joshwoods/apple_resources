

- RealityKit
- LoadRequest
-  min(by:) 

Instance Method

# min(by:)

Publishes the minimum value received from the upstream publisher, after it finishes.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func min(by areInIncreasingOrder: @escaping (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison
```

## Parameters 

`areInIncreasingOrder`  

A closure that receives two elements and returns true if they’re in increasing order.

## Return Value

A publisher that publishes the minimum value received from the upstream publisher, after the upstream publisher finishes.

## Discussion

Use `Publisher/min(by:)` to determine the minimum value in the stream of elements from an upstream publisher using a comparison operation you specify.

This operator is useful when the value received from the upstream publisher isn’t Comparable.

In the example below an array publishes enumeration elements representing playing card ranks. The `Publisher/min(by:)` operator compares the current and next elements using the `rawValue` property of each enumeration value in the user supplied closure and prints the minimum value found after publishing all of the elements.

```
enum Rank: Int {
    case ace = 1, two, three, four, five, six, seven, eight, nine, ten, jack, queen, king
}

let cards: [Rank] = [.five, .queen, .ace, .eight, .king]
cancellable = cards.publisher
    .min {
        return  $0.rawValue 

After this publisher receives a request for more than 0 items, it requests unlimited items from its upstream publisher.

## See Also

### Applying mathematical operations on elements

func count() -> Publishers.Count&lt;Self>

Publishes the number of elements received from the upstream publisher.

func max() -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, after it finishes.

func max(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided ordering closure.

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min() -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

