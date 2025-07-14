

- Combine
- CurrentValueSubject
-  replaceEmpty(with:) 

Instance Method

# replaceEmpty(with:)

Replaces an empty stream with the provided element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func replaceEmpty(with output: Self.Output) -> Publishers.ReplaceEmpty
```

## Parameters 

`output`  

An element to emit when the upstream publisher finishes without emitting any elements.

## Return Value

A publisher that replaces an empty stream with the provided output element.

## Discussion

Use replaceEmpty(with:) to provide a replacement element if the upstream publisher finishes without producing any elements.

In the example below, the empty `Double` array publisher doesn’t produce any elements, so replaceEmpty(with:) publishes `Double.nan` and finishes normally.

```
let numbers: [Double] = []
cancellable = numbers.publisher
    .replaceEmpty(with: Double.nan)
    .sink { print("\($0)", terminator: " ") }

// Prints "(nan)".
```

Conversely, providing a non-empty publisher publishes all elements and the publisher then terminates normally:

```
let otherNumbers: [Double] = [1.0, 2.0, 3.0]
cancellable2 = otherNumbers.publisher
    .replaceEmpty(with: Double.nan)
    .sink { print("\($0)", terminator: " ") }

// Prints: 1.0 2.0 3.0
```

## See Also

### Filtering Elements

func filter((Self.Output) -> Bool) -> Publishers.Filter&lt;Self>

Republishes all elements that match a provided closure.

func tryFilter((Self.Output) throws -> Bool) -> Publishers.TryFilter&lt;Self>

Republishes all elements that match a provided error-throwing closure.

func compactMap&lt;T>((Self.Output) -> T?) -> Publishers.CompactMap&lt;Self, T>

Calls a closure with each received element and publishes any returned optional that has a value.

func tryCompactMap&lt;T>((Self.Output) throws -> T?) -> Publishers.TryCompactMap&lt;Self, T>

Calls an error-throwing closure with each received element and publishes any returned optional that has a value.

func removeDuplicates() -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element.

func removeDuplicates(by: (Self.Output, Self.Output) -> Bool) -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided closure.

func tryRemoveDuplicates(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryRemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

func replaceError(with: Self.Output) -> Publishers.ReplaceError&lt;Self>

Replaces any errors in the stream with the provided element.

