

- Combine
- Publishers
- Publishers.DropWhile
-  min() 

Instance Method

# min()

Publishes the minimum value received from the upstream publisher, after it finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func min() -> Publishers.Comparison
```

Available when `Output` conforms to `Comparable`.

## Return Value

A publisher that publishes the minimum value received from the upstream publisher, after the upstream publisher finishes.

## Discussion

Use min(by:) to find the minimum value in a stream of elements from an upstream publisher.

In the example below, the min(by:) operator emits a value when the publisher finishes, that value is the minimum of the values received from upstream, which is `-1`.

```
let numbers = [-1, 0, 10, 5]
numbers.publisher
    .min()
    .sink { print("\($0)") }

// Prints: "-1"
```

After this publisher receives a request for more than 0 items, it requests unlimited items from its upstream publisher.

## See Also

### Applying Mathematical Operations on Elements

func count() -> Publishers.Count&lt;Self>

Publishes the number of elements received from the upstream publisher.

func max() -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, after it finishes.

func max(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided ordering closure.

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

