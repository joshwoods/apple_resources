

- RealityKit
- Scene
- Scene.Publisher
-  max(by:) 

Instance Method

# max(by:)

Publishes the maximum value received from the upstream publisher, using the provided ordering closure.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func max(by areInIncreasingOrder: @escaping (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison
```

## Parameters 

`areInIncreasingOrder`  

A closure that receives two elements and returns true if they’re in increasing order.

## Return Value

A publisher that publishes the maximum value received from the upstream publisher, after the upstream publisher finishes.

## Discussion

Use max(by:) to determine the maximum value of elements received from the upstream publisher based on an ordering closure you specify.

In the example below, an array publishes enumeration elements representing playing card ranks. The max(by:) operator compares the current and next elements using the `rawValue` property of each enumeration value in the user supplied closure and prints the maximum value found after publishing all of the elements.

```
enum Rank: Int {
    case ace = 1, two, three, four, five, six, seven, eight, nine, ten, jack, queen, king
}

let cards: [Rank] = [.five, .queen, .ace, .eight, .jack]
cancellable = cards.publisher
    .max {
        return  $0.rawValue > $1.rawValue
    }
    .sink { print("\($0)") }

// Prints: "queen"
```

After this publisher receives a request for more than 0 items, it requests unlimited items from its upstream publisher.

## See Also

### Applying mathematical operations on elements

func count() -> Publishers.Count&lt;Self>

Publishes the number of elements received from the upstream publisher.

func max() -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, after it finishes.

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min() -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func min(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

