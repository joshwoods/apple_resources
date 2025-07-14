

- Combine
- Empty
-  merge(with:) 

Instance Method

# merge(with:)

Combines elements from this publisher with those from another publisher, delivering an interleaved sequence of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func merge(with other: P) -> Publishers.Merge where P : Publisher, Self.Failure == P.Failure, Self.Output == P.Output
```

## Parameters 

`other`  

Another publisher.

## Return Value

A publisher that emits an event when either upstream publisher emits an event.

## Discussion

Use merge(with:) when you want to receive a new element whenever any of the upstream publishers emits an element. To receive tuples of the most-recent value from all the upstream publishers whenever any of them emit a value, use combineLatest(_:). To combine elements from multiple upstream publishers, use zip(_:).

In this example, as merge(with:) receives input from either upstream publisher, it republishes it to the downstream:

```
let publisher = PassthroughSubject()
let pub2 = PassthroughSubject()

cancellable = publisher
    .merge(with: pub2)
    .sink { print("\($0)", terminator: " " )}

publisher.send(2)
pub2.send(2)
publisher.send(3)
pub2.send(22)
publisher.send(45)
pub2.send(22)
publisher.send(17)

// Prints: "2 2 3 22 45 22 17"
```

The merged publisher continues to emit elements until all upstream publishers finish. If an upstream publisher produces an error, the merged publisher fails with that error.

