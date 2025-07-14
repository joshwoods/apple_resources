

- RealityKit
- Scene
- Scene.Publisher
-  merge(with:) 

Instance Method

# merge(with:)

Combines elements from this publisher with those from another publisher of the same type, delivering an interleaved sequence of elements.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func merge(with other: Self) -> Publishers.MergeMany
```

## Parameters 

`other`  

Another publisher of this publisher’s type.

## Return Value

A publisher that emits an event when either upstream publisher emits an event.

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

func merge&lt;B, C>(with: B, C) -> Publishers.Merge3&lt;Self, B, C>

Combines elements from this publisher with those from two other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D>(with: B, C, D) -> Publishers.Merge4&lt;Self, B, C, D>

Combines elements from this publisher with those from three other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E>(with: B, C, D, E) -> Publishers.Merge5&lt;Self, B, C, D, E>

Combines elements from this publisher with those from four other publishers, delivering an interleaved sequence of elements.

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

