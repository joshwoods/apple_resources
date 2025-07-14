

- Combine
- Publishers
- Publishers.Catch
-  last(where:) 

Instance Method

# last(where:)

Publishes the last element of a stream that satisfies a predicate closure, after upstream finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func last(where predicate: @escaping (Self.Output) -> Bool) -> Publishers.LastWhere
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value that indicates whether to publish the element.

## Return Value

A publisher that only publishes the last element satisfying the given predicate.

## Discussion

Use last(where:) when you need to republish only the last element of a stream that satisfies a closure you specify.

In the example below, a range publisher emits the last element that satisfies the closure’s criteria, then finishes normally:

```
let numbers = (-10...10)
cancellable = numbers.publisher
    .last { $0 

## See Also

### Selecting Specific Elements

func first() -> Publishers.First&lt;Self>

Publishes the first element of a stream, then finishes.

func first(where: (Self.Output) -> Bool) -> Publishers.FirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a predicate closure, then finishes normally.

func tryFirst(where: (Self.Output) throws -> Bool) -> Publishers.TryFirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a throwing predicate closure, then finishes normally.

func last() -> Publishers.Last&lt;Self>

Publishes the last element of a stream, after the stream finishes.

func tryLast(where: (Self.Output) throws -> Bool) -> Publishers.TryLastWhere&lt;Self>

Publishes the last element of a stream that satisfies an error-throwing predicate closure, after the stream finishes.

func output(at: Int) -> Publishers.Output&lt;Self>

Publishes a specific element, indicated by its index in the sequence of published elements.

func output&lt;R>(in: R) -> Publishers.Output&lt;Self>

Publishes elements specified by their range in the sequence of published elements.

