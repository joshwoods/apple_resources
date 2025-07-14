

- Combine
- Future
-  replaceNil(with:) 

Instance Method

# replaceNil(with:)

Replaces nil elements in the stream with the provided element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func replaceNil(with output: T) -> Publishers.Map where Self.Output == T?
```

## Parameters 

`output`  

The element to use when replacing `nil`.

## Return Value

A publisher that replaces `nil` elements from the upstream publisher with the provided element.

## Discussion

The replaceNil(with:) operator enables replacement of `nil` values in a stream with a substitute value. In the example below, a collection publisher contains a nil value. The replaceNil(with:) operator replaces this with `0.0`.

```
let numbers: [Double?] = [1.0, 2.0, nil, 3.0]
numbers.publisher
    .replaceNil(with: 0.0)
    .sink { print("\($0)", terminator: " ") }

// Prints: "Optional(1.0) Optional(2.0) Optional(0.0) Optional(3.0)"
```

## See Also

### Mapping Elements

func map&lt;T>((Self.Output) -> T) -> Publishers.Map&lt;Self, T>

Transforms all elements from the upstream publisher with a provided closure.

func tryMap&lt;T>((Self.Output) throws -> T) -> Publishers.TryMap&lt;Self, T>

Transforms all elements from the upstream publisher with a provided error-throwing closure.

func mapError&lt;E>((Self.Failure) -> E) -> Publishers.MapError&lt;Self, E>

Converts any failure from the upstream publisher into a new error.

func scan&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Scan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

func tryScan&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryScan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to an error-throwing closure along with the last value returned by the closure.

func setFailureType&lt;E>(to: E.Type) -> Publishers.SetFailureType&lt;Self, E>

Changes the failure type declared by the upstream publisher.

