

- Combine
- ObservableObjectPublisher
-  tryLast(where:) 

Instance Method

# tryLast(where:)

Publishes the last element of a stream that satisfies an error-throwing predicate closure, after the stream finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryLast(where predicate: @escaping (Self.Output) throws -> Bool) -> Publishers.TryLastWhere
```

## Parameters 

`predicate`  

A closure that takes an element as its parameter and returns a Boolean value that indicates whether to publish the element.

## Return Value

A publisher that only publishes the last element satisfying the given predicate.

## Discussion

Use tryLast(where:) when you need to republish the last element that satisfies an error-throwing closure you specify. If the predicate closure throws an error, the publisher fails.

In the example below, a publisher emits the last element that satisfies the error-throwing closure, then finishes normally:

```
struct RangeError: Error {}

let numbers = [-62, 1, 6, 10, 9, 22, 41, -1, 5]
cancellable = numbers.publisher
    .tryLast {
        guard 0 != 0  else {throw RangeError()}
        return true
    }
    .sink(
        receiveCompletion: { print ("completion: \($0)", terminator: " ") },
        receiveValue: { print ("\($0)", terminator: " ") }
    )
// Prints: "5 completion: finished"
// If instead the numbers array had contained a `0`, the `tryLast` operator would terminate publishing with a RangeError."
```

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

func last(where: (Self.Output) -> Bool) -> Publishers.LastWhere&lt;Self>

Publishes the last element of a stream that satisfies a predicate closure, after upstream finishes.

func output(at: Int) -> Publishers.Output&lt;Self>

Publishes a specific element, indicated by its index in the sequence of published elements.

func output&lt;R>(in: R) -> Publishers.Output&lt;Self>

Publishes elements specified by their range in the sequence of published elements.

