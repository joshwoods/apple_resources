

- Combine
- Publishers
- Publishers.Merge8
-  merge(with:\_:\_:\_:\_:) 

Instance Method

# merge(with:\_:\_:\_:\_:)

Combines elements from this publisher with those from five other publishers, delivering an interleaved sequence of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func merge(
    with b: B,
    _ c: C,
    _ d: D,
    _ e: E,
    _ f: F
) -> Publishers.Merge6 where B : Publisher, C : Publisher, D : Publisher, E : Publisher, F : Publisher, Self.Failure == B.Failure, Self.Output == B.Output, B.Failure == C.Failure, B.Output == C.Output, C.Failure == D.Failure, C.Output == D.Output, D.Failure == E.Failure, D.Output == E.Output, E.Failure == F.Failure, E.Output == F.Output
```

## Parameters 

`b`  

A second publisher.

`c`  

A third publisher.

`d`  

A fourth publisher.

`e`  

A fifth publisher.

`f`  

A sixth publisher.

## Return Value

A publisher that emits an event when any upstream publisher emits an event.

## Discussion

Use merge(with:_:_:_:_:_:) when you want to receive a new element whenever any of the upstream publishers emits an element. To receive tuples of the most-recent value from all the upstream publishers whenever any of them emit a value, use combineLatest(_:_:_:). To combine elements from multiple upstream publishers, use zip(_:_:_:).

In this example, as merge(with:_:_:_:_:_:) receives input from the upstream publishers, it republishes the interleaved elements to the downstream:

```
let pubA = PassthroughSubject()
let pubB = PassthroughSubject()
let pubC = PassthroughSubject()
let pubD = PassthroughSubject()
let pubE = PassthroughSubject()
let pubF = PassthroughSubject()

cancellable = pubA
    .merge(with: pubB, pubC, pubD, pubE, pubF)
    .sink { print("\($0)", terminator: " " ) }

pubA.send(1)
pubB.send(40)
pubC.send(90)
pubD.send(-1)
pubE.send(33)
pubF.send(44)

pubA.send(2)
pubB.send(50)
pubC.send(100)
pubD.send(-2)
pubE.send(33)
pubF.send(33)

//Prints: "1 40 90 -1 33 44 2 50 100 -2 33 33"
```

The merged publisher continues to emit elements until all upstream publishers finish. If an upstream publisher produces an error, the merged publisher fails with that error.

## See Also

### Republishing Elements from Multiple Publishers as an Interleaved Stream

func merge(with: Self) -> Publishers.MergeMany&lt;Self>

Combines elements from this publisher with those from another publisher of the same type, delivering an interleaved sequence of elements.

func merge&lt;B, C>(with: B, C) -> Publishers.Merge3&lt;Self, B, C>

Combines elements from this publisher with those from two other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D>(with: B, C, D) -> Publishers.Merge4&lt;Self, B, C, D>

Combines elements from this publisher with those from three other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E>(with: B, C, D, E) -> Publishers.Merge5&lt;Self, B, C, D, E>

Combines elements from this publisher with those from four other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F, G>(with: B, C, D, E, F, G) -> Publishers.Merge7&lt;Self, B, C, D, E, F, G>

Combines elements from this publisher with those from six other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F, G, H>(with: B, C, D, E, F, G, H) -> Publishers.Merge8&lt;Self, B, C, D, E, F, G, H>

Combines elements from this publisher with those from seven other publishers, delivering an interleaved sequence of elements.

