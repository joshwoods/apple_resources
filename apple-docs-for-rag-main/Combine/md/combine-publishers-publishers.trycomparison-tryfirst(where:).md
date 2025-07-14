

- Combine
- Publishers
- Publishers.TryComparison
-  tryFirst(where:) 

Instance Method

# tryFirst(where:)

Publishes the first element of a stream to satisfy a throwing predicate closure, then finishes normally.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryFirst(where predicate: @escaping (Self.Output) throws -> Bool) -> Publishers.TryFirstWhere
```

## Parameters 

`predicate`  

A closure that takes an element as a parameter and returns a Boolean value that indicates whether to publish the element.

## Return Value

A publisher that only publishes the first element of a stream that satisfies the predicate.

## Discussion

Use tryFirst(where:) when you need to republish only the first element of a stream that satisfies an error-throwing closure you specify. The publisher ignores all elements after the first. If this publisher doesn’t receive any elements, it finishes without publishing. If the predicate closure throws an error, the publisher fails.

In the example below, a range publisher emits the first element in the range then finishes normally:

```
let numberRange: ClosedRange = (-1...50)
numberRange.publisher
    .tryFirst {
        guard $0  = (100...200), the tryFirst operator would terminate publishing with a RangeError.
```

## See Also

### Selecting Specific Elements

func first() -> Publishers.First&lt;Self>

Publishes the first element of a stream, then finishes.

func first(where: (Self.Output) -> Bool) -> Publishers.FirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a predicate closure, then finishes normally.

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

