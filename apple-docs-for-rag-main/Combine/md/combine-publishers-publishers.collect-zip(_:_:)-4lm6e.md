

- Combine
- Publishers
- Publishers.Collect
-  zip(\_:\_:) 

Instance Method

# zip(\_:\_:)

Combines elements from another publisher and delivers a transformed output.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func zip(
    _ other: P,
    _ transform: @escaping (Self.Output, P.Output) -> T
) -> Publishers.Map, T> where P : Publisher, Self.Failure == P.Failure
```

## Parameters 

`other`  

Another publisher.

`transform`  

A closure that receives the most-recent value from each publisher and returns a new value to publish.

## Return Value

A publisher that uses the `transform` closure to emit new elements, produced by combining the most recent value from two upstream publishers.

## Discussion

Use zip(_:_:) to return a new publisher that combines the elements from two publishers using a transformation you specify to publish a new value to the downstream. The returned publisher waits until both publishers have emitted an event, then delivers the oldest unconsumed event from each publisher together that the operator uses in the transformation.

In this example, PassthroughSubject instances `numbersPub` and `lettersPub` emit values; zip(_:_:) receives the oldest value from each publisher, uses the `Int` from `numbersPub` and publishes a string that repeats the String from `lettersPub` that many times.

```
let numbersPub = PassthroughSubject()
let lettersPub = PassthroughSubject()
cancellable = numbersPub
    .zip(lettersPub) { anInt, aLetter in
        String(repeating: aLetter, count: anInt)
    }
    .sink { print("\($0)") }
numbersPub.send(1)     // numbersPub: 1      lettersPub:       zip output: 
numbersPub.send(2)     // numbersPub: 1,2    lettersPub:       zip output: 
numbersPub.send(3)     // numbersPub: 1,2,3  lettersPub:       zip output: 
lettersPub.send("A")   // numbersPub: 1,2,3  lettersPub: "A"   zip output: "A"
lettersPub.send("B")   // numbersPub: 2,3    lettersPub: "B"   zip output: "BB"
// Prints:
//  A
//  BB
```

If either upstream publisher finishes successfully or fails with an error, the zipped publisher does the same.

## See Also

### Collecting and Republishing the Oldest Unconsumed Elements from Multiple Publishers

func zip&lt;P>(P) -> Publishers.Zip&lt;Self, P>

Combines elements from another publisher and deliver pairs of elements as tuples.

func zip&lt;P, Q>(P, Q) -> Publishers.Zip3&lt;Self, P, Q>

Combines elements from two other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.Zip3&lt;Self, P, Q>, T>

Combines elements from two other publishers and delivers a transformed output.

func zip&lt;P, Q, R>(P, Q, R) -> Publishers.Zip4&lt;Self, P, Q, R>

Combines elements from three other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.Zip4&lt;Self, P, Q, R>, T>

Combines elements from three other publishers and delivers a transformed output.

