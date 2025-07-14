

- Combine
- Publishers
- Publishers.Zip4
-  count() 

Instance Method

# count()

Publishes the number of elements received from the upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func count() -> Publishers.Count
```

## Return Value

A publisher that consumes all elements until the upstream publisher finishes, then emits a single value with the total number of elements received.

## Discussion

Use count() to determine the number of elements received from the upstream publisher before it completes:

```
let numbers = (0...10)
cancellable = numbers.publisher
    .count()
    .sink { print("\($0)") }

// Prints: "11"
```

## See Also

### Applying Mathematical Operations on Elements

func max(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided ordering closure.

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

