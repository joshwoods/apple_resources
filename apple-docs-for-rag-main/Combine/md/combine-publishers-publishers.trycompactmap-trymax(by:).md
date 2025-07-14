

- Combine
- Publishers
- Publishers.TryCompactMap
-  tryMax(by:) 

Instance Method

# tryMax(by:)

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryMax(by areInIncreasingOrder: @escaping (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison
```

## Parameters 

`areInIncreasingOrder`  

A throwing closure that receives two elements and returns `true` if they’re in increasing order. If this closure throws, the publisher terminates with a Subscribers.Completion.failure(_:).

## Return Value

A publisher that publishes the maximum value received from the upstream publisher, after the upstream publisher finishes.

## Discussion

Use tryMax(by:) to determine the maximum value of elements received from the upstream publisher using an error-throwing closure you specify.

In the example below, an array publishes elements. The tryMax(by:) operator executes the error-throwing closure that throws when the `first` element is an odd number, terminating the publisher.

```
struct IllegalValueError: Error {}

let numbers: [Int]  = [0, 10, 6, 13, 22, 22]
cancellable = numbers.publisher
    .tryMax { first, second -> Bool in
        if (first % 2 != 0) {
            throw IllegalValueError()
        }
        return first > second
    }
    .sink(
        receiveCompletion: { print ("completion: \($0)") },
        receiveValue: { print ("value: \($0)") }
    )

// Prints: completion: failure(IllegalValueError())
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

func min() -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func min(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

