

- Swift
- Result
- Result.Publisher
-  collect(\_:) 

Instance Method

# collect(\_:)

Collects up to the specified number of elements, and then emits a single array of the collection.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func collect(_ count: Int) -> Publishers.CollectByCount
```

## Parameters 

`count`  

The maximum number of received elements to buffer before publishing.

## Return Value

A publisher that collects up to the specified number of elements, and then publishes them as an array.

## Discussion

Use collect(_:) to emit arrays of at most `count` elements from an upstream publisher. If the upstream publisher finishes before collecting the specified number of elements, the publisher sends an array of only the items it received. This may be fewer than `count` elements.

If the upstream publisher fails with an error, this publisher forwards the error to the downstream receiver instead of sending its output.

In the example below, the collect(_:) operator emits one partial and two full arrays based on the requested collection size of `5`:

```
let numbers = (0...10)
cancellable = numbers.publisher
    .collect(5)
    .sink { print("\($0), terminator: " "") }

// Prints "[0, 1, 2, 3, 4] [5, 6, 7, 8, 9] [10] "
```

Note

When this publisher receives a request for `.max(n)` elements, it requests `.max(count * n)` from the upstream publisher.

