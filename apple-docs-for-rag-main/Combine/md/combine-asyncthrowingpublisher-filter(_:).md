

- Combine
- AsyncThrowingPublisher
-  filter(\_:) 

Instance Method

# filter(\_:)

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

CombineSwiftiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
func filter(_ isIncluded: @escaping (Self.Element) async -> Bool) -> AsyncFilterSequence
```

## Parameters 

`isIncluded`  

A closure that takes an element of the asynchronous sequence as its argument and returns a Boolean value that indicates whether to include the element in the filtered sequence.

## Return Value

An asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `filter(_:)` method returns `true` for even values and `false` for odd values, thereby filtering out the odd values:

```
let stream = Counter(howHigh: 10)
    .filter { $0 % 2 == 0 }
for await number in stream {
    print(number, terminator: " ")
}
// Prints "2 4 6 8 10 "
```

