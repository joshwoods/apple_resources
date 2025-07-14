

- Combine
- Just
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

func map&lt;T>((Output) -> T) -> Just&lt;T>

func tryMap&lt;T>((Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func mapError&lt;E>((Just&lt;Output>.Failure) -> E) -> Result&lt;Output, E>.Publisher

func scan&lt;T>(T, (T, Output) -> T) -> Result&lt;T, Just&lt;Output>.Failure>.Publisher

func tryScan&lt;T>(T, (T, Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func setFailureType&lt;E>(to: E.Type) -> Result&lt;Output, E>.Publisher

