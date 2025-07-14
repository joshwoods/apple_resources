

- RealityKit
- Scene
- Scene.Publisher
-  merge(with:\_:\_:\_:) 

Instance Method

# merge(with:\_:\_:\_:)

Combines elements from this publisher with those from four other publishers, delivering an interleaved sequence of elements.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func merge(
    with b: B,
    _ c: C,
    _ d: D,
    _ e: E
) -> Publishers.Merge5 where B : Publisher, C : Publisher, D : Publisher, E : Publisher, Self.Failure == B.Failure, Self.Output == B.Output, B.Failure == C.Failure, B.Output == C.Output, C.Failure == D.Failure, C.Output == D.Output, D.Failure == E.Failure, D.Output == E.Output
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

## Return Value

A publisher that emits an event when any upstream publisher emits an event.

## Discussion

Use merge(with:_:_:_:) when you want to receive a new element whenever any of the upstream publishers emits an element. To receive tuples of the most-recent value from all the upstream publishers whenever any of them emit a value, use `Publisher/combineLatest(_:_:_:)-48buc`. To combine elements from multiple upstream publishers, use `Publisher/zip(_:_:_:)-16rcy`.

In this example, as merge(with:_:_:_:) receives input from the upstream publishers, it republishes the interleaved elements to the downstream:

```
 let pubA = PassthroughSubject()
 let pubB = PassthroughSubject()
 let pubC = PassthroughSubject()
 let pubD = PassthroughSubject()
 let pubE = PassthroughSubject()

 cancellable = pubA
     .merge(with: pubB, pubC, pubD, pubE)
     .sink { print("\($0)", terminator: " " ) }

 pubA.send(1)
 pubB.send(40)
 pubC.send(90)
 pubD.send(-1)
 pubE.send(33)
 pubA.send(2)
 pubB.send(50)
 pubC.send(100)
 pubD.send(-2)
 pubE.send(33)

 // Prints: "1 40 90 -1 33 2 50 100 -2 33"
```

The merged publisher continues to emit elements until all upstream publishers finish. If an upstream publisher produces an error, the merged publisher fails with that error.

## See Also

### Combining elements from multiple publishers

func combineLatest&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest&lt;Self, P>, T>

Subscribes to an additional publisher and invokes a closure upon receiving output from either publisher.

func combineLatest&lt;P>(P) -> Publishers.CombineLatest&lt;Self, P>

Subscribes to an additional publisher and publishes a tuple upon receiving output from either publisher.

func combineLatest&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest3&lt;Self, P, Q>, T>

Subscribes to two additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q>(P, Q) -> Publishers.CombineLatest3&lt;Self, P, Q>

Subscribes to two additional publishers and publishes a tuple upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest4&lt;Self, P, Q, R>, T>

Subscribes to three additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R>(P, Q, R) -> Publishers.CombineLatest4&lt;Self, P, Q, R>

Subscribes to three additional publishers and publishes a tuple upon receiving output from any of the publishers.

func merge(with: Self) -> Publishers.MergeMany&lt;Self>

Combines elements from this publisher with those from another publisher of the same type, delivering an interleaved sequence of elements.

func merge&lt;B, C>(with: B, C) -> Publishers.Merge3&lt;Self, B, C>

Combines elements from this publisher with those from two other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D>(with: B, C, D) -> Publishers.Merge4&lt;Self, B, C, D>

Combines elements from this publisher with those from three other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F>(with: B, C, D, E, F) -> Publishers.Merge6&lt;Self, B, C, D, E, F>

Combines elements from this publisher with those from five other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F, G>(with: B, C, D, E, F, G) -> Publishers.Merge7&lt;Self, B, C, D, E, F, G>

Combines elements from this publisher with those from six other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F, G, H>(with: B, C, D, E, F, G, H) -> Publishers.Merge8&lt;Self, B, C, D, E, F, G, H>

Combines elements from this publisher with those from seven other publishers, delivering an interleaved sequence of elements.

func zip&lt;P>(P) -> Publishers.Zip&lt;Self, P>

Combines elements from another publisher and deliver pairs of elements as tuples.

func zip&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.Zip&lt;Self, P>, T>

Combines elements from another publisher and delivers a transformed output.

func zip&lt;P, Q>(P, Q) -> Publishers.Zip3&lt;Self, P, Q>

Combines elements from two other publishers and delivers groups of elements as tuples.

