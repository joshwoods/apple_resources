

- Combine
- Publishers
- Publishers.Merge7
-  combineLatest(\_:\_:\_:\_:) 

Instance Method

# combineLatest(\_:\_:\_:\_:)

Subscribes to three additional publishers and invokes a closure upon receiving output from any of the publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func combineLatest(
    _ publisher1: P,
    _ publisher2: Q,
    _ publisher3: R,
    _ transform: @escaping (Self.Output, P.Output, Q.Output, R.Output) -> T
) -> Publishers.Map, T> where P : Publisher, Q : Publisher, R : Publisher, Self.Failure == P.Failure, P.Failure == Q.Failure, Q.Failure == R.Failure
```

## Parameters 

`publisher1`  

A second publisher to combine with the first publisher.

`publisher2`  

A third publisher to combine with the first publisher.

`publisher3`  

A fourth publisher to combine with the first publisher.

`transform`  

A closure that receives the most-recent value from each publisher and returns a new value to publish.

## Return Value

A publisher that receives and combines elements from this publisher and three other publishers.

## Discussion

Use combineLatest(_:_:_:_:) when you need to combine the current and 3 additional publishers and transform the values using a closure in which you specify the published elements, to publish a new element.

Tip

The combined publisher doesn’t produce elements until each of its upstream publishers publishes at least one element.

The combined publisher passes through any requests to *all* upstream publishers. However, it still obeys the demand-fulfilling rule of only sending the request amount downstream. If the demand isn’t unlimited, it drops values from upstream publishers. It implements this by using a buffer size of 1 for each upstream, and holds the most-recent value in each buffer.

All upstream publishers need to finish for this publisher to finish. If an upstream publisher never publishes a value, this publisher never finishes.

In the example below, as combineLatest(_:_:_:_:) receives the most-recent values published by four publishers, multiplies them together, and republishes the result:

```
let pub = PassthroughSubject()
let pub2 = PassthroughSubject()
let pub3 = PassthroughSubject()
let pub4 = PassthroughSubject()

cancellable = pub
    .combineLatest(pub2, pub3, pub4) { firstValue, secondValue, thirdValue, fourthValue in
        return firstValue * secondValue * thirdValue * fourthValue
    }
    .sink { print("Result: \($0).") }

pub.send(1)
pub.send(2)
pub2.send(2)
pub3.send(9)
pub4.send(1)

pub.send(3)
pub2.send(12)
pub.send(13)
pub3.send(19)

// Prints:
//  Result: 36.     // pub = 2,  pub2 = 2,   pub3 = 9,  pub4 = 1
//  Result: 54.     // pub = 3,  pub2 = 2,   pub3 = 9,  pub4 = 1
//  Result: 324.    // pub = 3,  pub2 = 12,  pub3 = 9,  pub4 = 1
//  Result: 1404.   // pub = 13, pub2 = 12,  pub3 = 9,  pub4 = 1
//  Result: 2964.   // pub = 13, pub2 = 12,  pub3 = 19, pub4 = 1
```

## See Also

### Collecting and Republishing the Latest Elements from Multiple Publishers

func combineLatest&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest&lt;Self, P>, T>

Subscribes to an additional publisher and invokes a closure upon receiving output from either publisher.

func combineLatest&lt;P>(P) -> Publishers.CombineLatest&lt;Self, P>

Subscribes to an additional publisher and publishes a tuple upon receiving output from either publisher.

func combineLatest&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest3&lt;Self, P, Q>, T>

Subscribes to two additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q>(P, Q) -> Publishers.CombineLatest3&lt;Self, P, Q>

Subscribes to two additional publishers and publishes a tuple upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R>(P, Q, R) -> Publishers.CombineLatest4&lt;Self, P, Q, R>

Subscribes to three additional publishers and publishes a tuple upon receiving output from any of the publishers.

