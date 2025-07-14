

- Swift
- AsyncSequence
-  filter(\_:) 

Instance Method

# filter(\_:)

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given error-throwing predicate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func filter(_ isIncluded: @escaping (Self.Element) async throws -> Bool) -> AsyncThrowingFilterSequence
```

## Parameters 

`isIncluded`  

An error-throwing closure that takes an element of the asynchronous sequence as its argument and returns a Boolean value that indicates whether to include the element in the filtered sequence.

## Return Value

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate. If the predicate throws an error, the sequence contains only values produced prior to the error.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `filter(_:)` method returns `true` for even values and `false` for odd values, thereby filtering out the odd values, but also throws an error for values divisible by 5:

```
do {
    let stream = Counter(howHigh: 10)
        .filter {
            if $0 % 5 == 0 {
                throw MyError()
            }
            return $0 % 2 == 0
        }
    for try await number in stream {
        print(number, terminator: " ")
    }
} catch {
    print("Error: \(error)")
}
// Prints "2 4 Error: MyError() "
```

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

func drop(while: (Self.Element) async throws -> Bool) -> AsyncThrowingDropWhileSequence&lt;Self>

Omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

struct AsyncThrowingDropWhileSequence

An asynchronous sequence which omits elements from the base sequence until a given error-throwing closure returns false, after which it passes through all remaining elements.

func filter((Self.Element) async -> Bool) -> AsyncFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

struct AsyncFilterSequence

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy a given predicate.

struct AsyncThrowingFilterSequence

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given error-throwing predicate.

