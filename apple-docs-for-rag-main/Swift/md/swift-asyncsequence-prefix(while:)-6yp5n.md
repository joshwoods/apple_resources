

- Swift
- AsyncSequence
-  prefix(while:) 

Instance Method

# prefix(while:)

Returns an asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given error-throwing predicate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func prefix(while predicate: @escaping (Self.Element) async throws -> Bool) rethrows -> AsyncThrowingPrefixWhileSequence
```

## Parameters 

`predicate`  

A error-throwing closure that takes an element of the asynchronous sequence as its argument and returns a Boolean value that indicates whether to include the element in the modified sequence.

## Return Value

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate. If the predicate throws an error, the sequence contains only values produced prior to the error.

## Discussion

Use `prefix(while:)` to produce values while elements from the base sequence meet a condition you specify. The modified sequence ends when the predicate closure returns `false` or throws an error.

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `prefix(_:)` method causes the modified sequence to pass through values less than `8`, but throws an error when it receives a value that’s divisible by `5`:

```
do {
    let stream = try Counter(howHigh: 10)
        .prefix {
            if $0 % 5 == 0 {
                throw MyError()
            }
            return $0 

## See Also

### Selecting Elements

func prefix(Int) -> AsyncPrefixSequence&lt;Self>

Returns an asynchronous sequence, up to the specified maximum length, containing the initial elements of the base asynchronous sequence.

struct AsyncPrefixSequence

An asynchronous sequence, up to a specified maximum length, containing the initial elements of a base asynchronous sequence.

func prefix(while: (Self.Element) async -> Bool) rethrows -> AsyncPrefixWhileSequence&lt;Self>

Returns an asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given predicate.

struct AsyncPrefixWhileSequence

An asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy a given predicate.

struct AsyncThrowingPrefixWhileSequence

An asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given error-throwing predicate.

