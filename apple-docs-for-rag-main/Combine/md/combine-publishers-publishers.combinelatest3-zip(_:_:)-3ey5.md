

- Combine
- Publishers
- Publishers.CombineLatest3
-  zip(\_:\_:) 

Instance Method

# zip(\_:\_:)

Combines elements from two other publishers and delivers groups of elements as tuples.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func zip(
    _ publisher1: P,
    _ publisher2: Q
) -> Publishers.Zip3 where P : Publisher, Q : Publisher, Self.Failure == P.Failure, P.Failure == Q.Failure
```

## Parameters 

`publisher1`  

A second publisher.

`publisher2`  

A third publisher.

## Return Value

A publisher that emits groups of elements from the upstream publishers as tuples.

## Discussion

Use zip(_:_:) to return a new publisher that combines the elements from two additional publishers to publish a tuple to the downstream. The returned publisher waits until all three publishers have emitted an event, then delivers the oldest unconsumed event from each publisher as a tuple to the subscriber.

In this example, `numbersPub`, `lettersPub` and `emojiPub` are each a PassthroughSubject; zip(_:_:) receives the oldest unconsumed value from each publisher and combines them into a tuple that it republishes to the downstream:

```
let numbersPub = PassthroughSubject()
let lettersPub = PassthroughSubject()
let emojiPub = PassthroughSubject()

cancellable = numbersPub
    .zip(lettersPub, emojiPub)
    .sink { print("\($0)") }
numbersPub.send(1)     // numbersPub: 1      lettersPub:          emojiPub:        zip output: 
numbersPub.send(2)     // numbersPub: 1,2    lettersPub:          emojiPub:        zip output: 
numbersPub.send(3)     // numbersPub: 1,2,3  lettersPub:          emojiPub:        zip output: 
lettersPub.send("A")   // numbersPub: 1,2,3  lettersPub: "A"      emojiPub:        zip output: 
emojiPub.send("😀")    // numbersPub: 2,3    lettersPub: "A"      emojiPub: "😀"   zip output: (1, "A", "😀")
lettersPub.send("B")   // numbersPub: 2,3    lettersPub: "B"      emojiPub:        zip output: 
emojiPub.send("🥰")    // numbersPub: 3      lettersPub:          emojiPub:        zip output: (2, "B", "🥰")

// Prints:
//  (1, "A", "😀")
//  (2, "B", "🥰")
```

If any upstream publisher finishes successfully or fails with an error, so too does the zipped publisher.

## See Also

### Collecting and Republishing the Oldest Unconsumed Elements from Multiple Publishers

func zip&lt;P>(P) -> Publishers.Zip&lt;Self, P>

Combines elements from another publisher and deliver pairs of elements as tuples.

func zip&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.Zip&lt;Self, P>, T>

Combines elements from another publisher and delivers a transformed output.

func zip&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.Zip3&lt;Self, P, Q>, T>

Combines elements from two other publishers and delivers a transformed output.

func zip&lt;P, Q, R>(P, Q, R) -> Publishers.Zip4&lt;Self, P, Q, R>

Combines elements from three other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.Zip4&lt;Self, P, Q, R>, T>

Combines elements from three other publishers and delivers a transformed output.

