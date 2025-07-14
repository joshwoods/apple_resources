

- Combine
- Publishers
- Publishers.Print
-  output(in:) 

Instance Method

# output(in:)

Publishes elements specified by their range in the sequence of published elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func output(in range: R) -> Publishers.Output where R : RangeExpression, R.Bound == Int
```

## Parameters 

`range`  

A range that indicates which elements to publish.

## Return Value

A publisher that publishes elements specified by a range.

## Discussion

Use output(in:) to republish a range indices you specify in the published stream. After publishing all elements, the publisher finishes normally. If the publisher completes normally or with an error before producing all the elements in the range, it doesn’t publish the remaining elements.

In the example below, an array publisher emits the subset of elements at the indices in the specified range:

```
let numbers = [1, 1, 2, 2, 2, 3, 4, 5, 6]
numbers.publisher
    .output(in: (3...5))
    .sink { print("\($0)", terminator: " ") }

// Prints: "2 2 3"
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

func tryLast(where: (Self.Output) throws -> Bool) -> Publishers.TryLastWhere&lt;Self>

Publishes the last element of a stream that satisfies an error-throwing predicate closure, after the stream finishes.

func output(at: Int) -> Publishers.Output&lt;Self>

Publishes a specific element, indicated by its index in the sequence of published elements.

