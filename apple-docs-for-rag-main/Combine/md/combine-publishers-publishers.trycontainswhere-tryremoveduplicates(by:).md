

- Combine
- Publishers
- Publishers.TryContainsWhere
-  tryRemoveDuplicates(by:) 

Instance Method

# tryRemoveDuplicates(by:)

Publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryRemoveDuplicates(by predicate: @escaping (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryRemoveDuplicates
```

## Parameters 

`predicate`  

A closure to evaluate whether two elements are equivalent, for purposes of filtering. Return `true` from this closure to indicate that the second element is a duplicate of the first. If this closure throws an error, the publisher terminates with the thrown error.

## Return Value

A publisher that consumes — rather than publishes — duplicate elements.

## Discussion

Use tryRemoveDuplicates(by:) to remove repeating elements from an upstream publisher based upon the evaluation of elements using an error-throwing closure you provide. If your closure throws an error, the publisher terminates with the error.

In the example below, the closure provided to tryRemoveDuplicates(by:) returns `true` when two consecutive elements are equal, thereby filtering out `0`, `1`, `2`, and `3`. However, the closure throws an error when it encounters `4`. The publisher then terminates with this error.

```
struct BadValuesError: Error {}
let numbers = [0, 0, 0, 0, 1, 2, 2, 3, 3, 3, 4, 4, 4, 4]
cancellable = numbers.publisher
    .tryRemoveDuplicates { first, second -> Bool in
        if (first == 4 && second == 4) {
            throw BadValuesError()
        }
        return first == second
    }
    .sink(
        receiveCompletion: { print ("\($0)") },
        receiveValue: { print ("\($0)", terminator: " ") }
     )

 // Prints: "0 1 2 3 4 failure(BadValuesError()"
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

func replaceEmpty(with: Self.Output) -> Publishers.ReplaceEmpty&lt;Self>

Replaces an empty stream with the provided element.

func replaceError(with: Self.Output) -> Publishers.ReplaceError&lt;Self>

Replaces any errors in the stream with the provided element.

