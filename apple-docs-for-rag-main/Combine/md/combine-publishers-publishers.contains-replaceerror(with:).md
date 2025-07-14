

- Combine
- Publishers
- Publishers.Contains
-  replaceError(with:) 

Instance Method

# replaceError(with:)

Replaces any errors in the stream with the provided element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func replaceError(with output: Self.Output) -> Publishers.ReplaceError
```

## Parameters 

`output`  

An element to emit when the upstream publisher fails.

## Return Value

A publisher that replaces an error from the upstream publisher with the provided output element.

## Discussion

If the upstream publisher fails with an error, this publisher emits the provided element, then finishes normally.

In the example below, a publisher of strings fails with a `MyError` instance, which sends a failure completion downstream. The replaceError(with:) operator handles the failure by publishing the string `(replacement element)` and completing normally.

```
struct MyError: Error {}
let fail = Fail(error: MyError())
cancellable = fail
    .replaceError(with: "(replacement element)")
    .sink(
        receiveCompletion: { print ("\($0)") },
        receiveValue: { print ("\($0)", terminator: " ") }
    )

// Prints: "(replacement element) finished".
```

This replaceError(with:) functionality is useful when you want to handle an error by sending a single replacement element and end the stream. Use catch(_:) to recover from an error and provide a replacement publisher to continue providing elements to the downstream subscriber.

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

func replaceEmpty(with: Self.Output) -> Publishers.ReplaceEmpty&lt;Self>

Replaces an empty stream with the provided element.

