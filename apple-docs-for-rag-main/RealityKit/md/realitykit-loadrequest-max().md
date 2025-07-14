

- RealityKit
- LoadRequest
-  max() 

Instance Method

# max()

Publishes the maximum value received from the upstream publisher, after it finishes.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func max() -> Publishers.Comparison
```

Available when `Output` conforms to `Comparable`.

## Return Value

A publisher that publishes the maximum value received from the upstream publisher, after the upstream publisher finishes.

## Discussion

Use `Publisher/max()` to determine the maximum value in the stream of elements from an upstream publisher.

In the example below, the `Publisher/max()` operator emits a value when the publisher finishes, that value is the maximum of the values received from upstream, which is `10`.

```
let numbers = [0, 10, 5]
cancellable = numbers.publisher
    .max()
    .sink { print("\($0)") }

// Prints: "10"
```

After this publisher receives a request for more than 0 items, it requests unlimited items from its upstream publisher.

## See Also

### Applying mathematical operations on elements

func count() -> Publishers.Count&lt;Self>

Publishes the number of elements received from the upstream publisher.

func max(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided ordering closure.

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min() -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func min(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

