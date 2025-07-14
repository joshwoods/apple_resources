

- Combine
- Publishers
- Publishers.Multicast
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

## See Also

### Selecting Specific Elements

func first(where: (Self.Output) -> Bool) -> Publishers.FirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a predicate closure, then finishes normally.

func tryFirst(where: (Self.Output) throws -> Bool) -> Publishers.TryFirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a throwing predicate closure, then finishes normally.

func last() -> Publishers.Last&lt;Self>

Publishes the last element of a stream, after the stream finishes.

func last(where: (Self.Output) -> Bool) -> Publishers.LastWhere&lt;Self>

Publishes the last element of a stream that satisfies a predicate closure, after upstream finishes.

func tryLast(where: (Self.Output) throws -> Bool) -> Publishers.TryLastWhere&lt;Self>

Publishes the last element of a stream that satisfies an error-throwing predicate closure, after the stream finishes.

func output(at: Int) -> Publishers.Output&lt;Self>

Publishes a specific element, indicated by its index in the sequence of published elements.

func output&lt;R>(in: R) -> Publishers.Output&lt;Self>

Publishes elements specified by their range in the sequence of published elements.

