

- Swift
- AsyncSequence
-  dropFirst(\_:) 

Instance Method

# dropFirst(\_:)

Omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func dropFirst(_ count: Int = 1) -> AsyncDropFirstSequence
```

## Parameters 

`count`  

The number of elements to drop from the beginning of the sequence. `count` must be greater than or equal to zero.

## Return Value

An asynchronous sequence that drops the first `count` elements from the base sequence.

## Discussion

Use `dropFirst(_:)` when you want to drop the first *n* elements from the base sequence and pass through the remaining elements.

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `dropFirst(_:)` method causes the modified sequence to ignore the values `1` through `3`, and instead emit `4` through `10`:

```
for await number in Counter(howHigh: 10).dropFirst(3) {
    print(number, terminator: " ")
}
// Prints "4 5 6 7 8 9 10 "
```

If the number of elements to drop exceeds the number of elements in the sequence, the result is an empty sequence.

## See Also

### Excluding Elements

struct AsyncDropFirstSequence

An asynchronous sequence which omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

func drop(while: (Self.Element) async -> Bool) -> AsyncDropWhileSequence&lt;Self>

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

struct AsyncDropWhileSequence

An asynchronous sequence which omits elements from the base sequence until a given closure returns false, after which it passes through all remaining elements.

func drop(while: (Self.Element) async throws -> Bool) -> AsyncThrowingDropWhileSequence&lt;Self>

Omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

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

