

- Combine
- Just
-  first() 

Instance Method

# first()

Publishes the first element of a stream, then finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func first() -> Publishers.First
```

## Return Value

A publisher that only publishes the first element of a stream.

## Discussion

Use first() to publish just the first element from an upstream publisher, then finish normally. The first() operator requests unlimited from its upstream as soon as downstream requests at least one element. If the upstream completes before first() receives any elements, it completes without emitting any values.

In this example, the first() publisher republishes the first element received from the sequence publisher, `-10`, then finishes normally.

```
let numbers = (-10...10)
cancellable = numbers.publisher
    .first()
    .sink { print("\($0)") }

// Print: "-10"
```

