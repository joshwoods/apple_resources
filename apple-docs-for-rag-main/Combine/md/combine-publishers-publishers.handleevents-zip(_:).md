

- Combine
- Publishers
- Publishers.HandleEvents
-  zip(\_:) 

Instance Method

# zip(\_:)

Combines elements from another publisher and deliver pairs of elements as tuples.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func zip(_ other: P) -> Publishers.Zip where P : Publisher, Self.Failure == P.Failure
```

## Parameters 

`other`  

Another publisher.

## Return Value

A publisher that emits pairs of elements from the upstream publishers as tuples.

## Discussion

Use zip(_:) to combine the latest elements from two publishers and emit a tuple to the downstream. The returned publisher waits until both publishers have emitted an event, then delivers the oldest unconsumed event from each publisher together as a tuple to the subscriber.

Much like a zipper or zip fastener on a piece of clothing pulls together rows of teeth to link the two sides, zip(_:) combines streams from two different publishers by linking pairs of elements from each side.

In this example, `numbers` and `letters` are PassthroughSubjects that emit values; once zip(_:) receives one value from each, it publishes the pair as a tuple to the downstream subscriber. It then waits for the next pair of values.

```
 let numbersPub = PassthroughSubject()
 let lettersPub = PassthroughSubject()

 cancellable = numbersPub
     .zip(lettersPub)
     .sink { print("\($0)") }
 numbersPub.send(1)    // numbersPub: 1      lettersPub:        zip output: 
 numbersPub.send(2)    // numbersPub: 1,2    lettersPub:        zip output: 
 letters.send("A")     // numbers: 1,2       letters:"A"        zip output: 
 numbers.send(3)       // numbers: 1,2,3     letters:           zip output: (1,"A")
 letters.send("B")     // numbers: 1,2,3     letters: "B"       zip output: (2,"B")

 // Prints:
 //  (1, "A")
 //  (2, "B")
```

If either upstream publisher finishes successfully or fails with an error, the zipped publisher does the same.

## See Also

### Collecting and Republishing the Oldest Unconsumed Elements from Multiple Publishers

func zip&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.Zip&lt;Self, P>, T>

Combines elements from another publisher and delivers a transformed output.

func zip&lt;P, Q>(P, Q) -> Publishers.Zip3&lt;Self, P, Q>

Combines elements from two other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.Zip3&lt;Self, P, Q>, T>

Combines elements from two other publishers and delivers a transformed output.

func zip&lt;P, Q, R>(P, Q, R) -> Publishers.Zip4&lt;Self, P, Q, R>

Combines elements from three other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.Zip4&lt;Self, P, Q, R>, T>

Combines elements from three other publishers and delivers a transformed output.

