

- Swift
- AsyncSequence
-  drop(while:) 

Instance Method

# drop(while:)

Omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func drop(while predicate: @escaping (Self.Element) async throws -> Bool) -> AsyncThrowingDropWhileSequence
```

## Parameters 

`predicate`  

An error-throwing closure that takes an element as a parameter and returns a Boolean value indicating whether to drop the element from the modified sequence.

## Return Value

An asynchronous sequence that skips over values until the provided closure returns `false` or throws an error.

## Discussion

Use `drop(while:)` to omit elements from an asynchronous sequence until the element received meets a condition you specify. If the closure you provide throws an error, the sequence produces no elements and throws the error instead.

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The predicate passed to the `drop(while:)` method throws an error if it encounters an even number, and otherwise returns `true` while it receives elements less than `5`. Because the predicate throws when it receives `2` from the base sequence, this example throws without ever printing anything.

```
do {
    let stream = Counter(howHigh: 10)
        .drop {
            if $0 % 2 == 0 {
                throw EvenError()
            }
            return $0 

After the predicate returns `false`, the sequence never executes it again, and from then on the sequence passes through elements from its underlying sequence. A predicate that throws an error also never executes again.

## See Also

### Excluding Elements

func dropFirst(Int) -> AsyncDropFirstSequence&lt;Self>

Omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

struct AsyncDropFirstSequence

An asynchronous sequence which omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

func drop(while: (Self.Element) async -> Bool) -> AsyncDropWhileSequence&lt;Self>

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

struct AsyncDropWhileSequence

An asynchronous sequence which omits elements from the base sequence until a given closure returns false, after which it passes through all remaining elements.

struct AsyncThrowingDropWhileSequence

An asynchronous sequence which omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

func filter((Self.Element) async -> Bool) -> AsyncFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

struct AsyncFilterSequence

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy a given predicate.

func filter((Self.Element) async throws -> Bool) -> AsyncThrowingFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given error-throwing predicate.

struct AsyncThrowingFilterSequence

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given error-throwing predicate.

