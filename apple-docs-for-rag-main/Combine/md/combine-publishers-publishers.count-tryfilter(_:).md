

- Combine
- Publishers
- Publishers.Count
-  tryFilter(\_:) 

Instance Method

# tryFilter(\_:)

Republishes all elements that match a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryFilter(_ isIncluded: @escaping (Self.Output) throws -> Bool) -> Publishers.TryFilter
```

## Parameters 

`isIncluded`  

A closure that takes one element and returns a Boolean value that indicated whether to republish the element or throws an error.

## Return Value

A publisher that republishes all elements that satisfy the closure.

## Discussion

Use tryFilter(_:) to filter elements evaluated in an error-throwing closure. If the `isIncluded` closure throws an error, the publisher fails with that error.

In the example below, tryFilter(_:) checks to see if the element provided by the publisher is zero, and throws a `ZeroError` before terminating the publisher with the thrown error. Otherwise, it republishes the element only if it’s even:

```
struct ZeroError: Error {}

let numbers: [Int] = [1, 2, 3, 4, 0, 5]
cancellable = numbers.publisher
    .tryFilter{
        if $0 == 0 {
            throw ZeroError()
        } else {
            return $0 % 2 == 0
        }
    }
    .sink(
        receiveCompletion: { print ("\($0)") },
        receiveValue: { print ("\($0)", terminator: " ") }
     )

// Prints: "2 4 failure(DivisionByZeroError())".
```

## See Also

### Filtering Elements

func filter((Self.Output) -> Bool) -> Publishers.Filter&lt;Self>

Republishes all elements that match a provided closure.

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

func replaceError(with: Self.Output) -> Publishers.ReplaceError&lt;Self>

Replaces any errors in the stream with the provided element.

