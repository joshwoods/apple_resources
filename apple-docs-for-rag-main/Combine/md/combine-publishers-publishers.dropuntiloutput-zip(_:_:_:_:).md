

- Combine
- Publishers
- Publishers.DropUntilOutput
-  zip(\_:\_:\_:\_:) 

Instance Method

# zip(\_:\_:\_:\_:)

Combines elements from three other publishers and delivers a transformed output.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func zip(
    _ publisher1: P,
    _ publisher2: Q,
    _ publisher3: R,
    _ transform: @escaping (Self.Output, P.Output, Q.Output, R.Output) -> T
) -> Publishers.Map, T> where P : Publisher, Q : Publisher, R : Publisher, Self.Failure == P.Failure, P.Failure == Q.Failure, Q.Failure == R.Failure
```

## Parameters 

`publisher1`  

A second publisher.

`publisher2`  

A third publisher.

`publisher3`  

A fourth publisher.

`transform`  

A closure that receives the most-recent value from each publisher and returns a new value to publish.

## Return Value

A publisher that uses the `transform` closure to emit new elements, produced by combining the most recent value from four upstream publishers.

## Discussion

Use zip(_:_:_:_:) to return a new publisher that combines the elements from three other publishers using a transformation you specify to publish a new value to the downstream subscriber. The returned publisher waits until all four publishers have emitted an event, then delivers the oldest unconsumed event from each publisher together that the operator uses in the transformation.

In this example, the PassthroughSubject publishers, `numbersPub`, `fractionsPub`, `lettersPub`, and `emojiPub` emit values. The zip(_:_:_:_:) operator receives the oldest value from each publisher and uses the `Int` from `numbersPub` and publishes a string that repeats the String from `lettersPub` and `emojiPub` that many times and prints out the value in `fractionsPub`.

```
let numbersPub = PassthroughSubject()      // first publisher
let lettersPub = PassthroughSubject()   // second
let emojiPub = PassthroughSubject()     // third
let fractionsPub  = PassthroughSubject()// fourth

cancellable = numbersPub
    .zip(lettersPub, emojiPub, fractionsPub) { anInt, aLetter, anEmoji, aFraction  in
        ("\(String(repeating: anEmoji, count: anInt)) \(String(repeating: aLetter, count: anInt)) \(aFraction)")
    }
    .sink { print("\($0)") }

numbersPub.send(1)         // numbersPub: 1       lettersPub:          emojiPub:          zip output: 
numbersPub.send(2)         // numbersPub: 1,2     lettersPub:          emojiPub:          zip output: 
numbersPub.send(3)         // numbersPub: 1,2,3   lettersPub:          emojiPub:          zip output: 
fractionsPub.send(0.1)     // numbersPub: 1,2,3   lettersPub: "A"      emojiPub:          zip output: 
lettersPub.send("A")       // numbersPub: 1,2,3   lettersPub: "A"      emojiPub:          zip output: 
emojiPub.send("😀")        // numbersPub: 1,2,3   lettersPub: "A"      emojiPub:"😀"      zip output: "😀 A"
lettersPub.send("B")       // numbersPub: 2,3     lettersPub: "B"      emojiPub:          zip output: 
fractionsPub.send(0.8)     // numbersPub: 2,3     lettersPub: "A"      emojiPub:          zip output: 
emojiPub.send("🥰")        // numbersPub: 3       lettersPub: "B"      emojiPub:          zip output: "🥰🥰 BB"
// Prints:
//1 😀 A 0.1
//2 🥰🥰 BB 0.8
```

If any upstream publisher finishes successfully or fails with an error, so too does the zipped publisher.

## See Also

### Collecting and Republishing the Oldest Unconsumed Elements from Multiple Publishers

func zip&lt;P>(P) -> Publishers.Zip&lt;Self, P>

Combines elements from another publisher and deliver pairs of elements as tuples.

func zip&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.Zip&lt;Self, P>, T>

Combines elements from another publisher and delivers a transformed output.

func zip&lt;P, Q>(P, Q) -> Publishers.Zip3&lt;Self, P, Q>

Combines elements from two other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.Zip3&lt;Self, P, Q>, T>

Combines elements from two other publishers and delivers a transformed output.

func zip&lt;P, Q, R>(P, Q, R) -> Publishers.Zip4&lt;Self, P, Q, R>

Combines elements from three other publishers and delivers groups of elements as tuples.

