

- Combine
- Publishers
- Publishers.Multicast
-  combineLatest(\_:\_:\_:) 

Instance Method

# combineLatest(\_:\_:\_:)

Subscribes to two additional publishers and invokes a closure upon receiving output from any of the publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func combineLatest(
    _ publisher1: P,
    _ publisher2: Q,
    _ transform: @escaping (Self.Output, P.Output, Q.Output) -> T
) -> Publishers.Map, T> where P : Publisher, Q : Publisher, Self.Failure == P.Failure, P.Failure == Q.Failure
```

## Parameters 

`publisher1`  

A second publisher to combine with the first publisher.

`publisher2`  

A third publisher to combine with the first publisher.

`transform`  

A closure that receives the most-recent value from each publisher and returns a new value to publish.

## Return Value

A publisher that receives and combines elements from this publisher and two other publishers.

## Discussion

Use `combineLatest(_:,_:)` to combine the current and two additional publishers and transform them using a closure you specify to publish a new value to the downstream.

Tip

The combined publisher doesn’t produce elements until each of its upstream publishers publishes at least one element.

The combined publisher passes through any requests to *all* upstream publishers. However, it still obeys the demand-fulfilling rule of only sending the request amount downstream. If the demand isn’t `.unlimited`, it drops values from upstream publishers. It implements this by using a buffer size of 1 for each upstream, and holds the most-recent value in each buffer. All upstream publishers need to finish for this publisher to finish. If an upstream publisher never publishes a value, this publisher never finishes. If any of the combined publishers terminates with a failure, this publisher also fails.

In the example below, `combineLatest()` receives the most-recent values published by three publishers, multiplies them together, and republishes the result:

```
let pub = PassthroughSubject()
let pub2 = PassthroughSubject()
let pub3 = PassthroughSubject()

cancellable = pub
    .combineLatest(pub2, pub3) { firstValue, secondValue, thirdValue in
        return firstValue * secondValue * thirdValue
    }
    .sink { print("Result: \($0).") }

pub.send(1)
pub.send(2)
pub2.send(2)
pub3.send(10)

pub.send(9)
pub3.send(4)
pub2.send(12)

// Prints:
//  Result: 40.     // pub = 2, pub2 = 2, pub3 = 10
//  Result: 180.    // pub = 9, pub2 = 2, pub3 = 10
//  Result: 72.     // pub = 9, pub2 = 2, pub3 = 4
//  Result: 432.    // pub = 9, pub2 = 12, pub3 = 4
```

## See Also

### Collecting and Republishing the Latest Elements from Multiple Publishers

func combineLatest&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest&lt;Self, P>, T>

Subscribes to an additional publisher and invokes a closure upon receiving output from either publisher.

func combineLatest&lt;P>(P) -> Publishers.CombineLatest&lt;Self, P>

Subscribes to an additional publisher and publishes a tuple upon receiving output from either publisher.

func combineLatest&lt;P, Q>(P, Q) -> Publishers.CombineLatest3&lt;Self, P, Q>

Subscribes to two additional publishers and publishes a tuple upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest4&lt;Self, P, Q, R>, T>

Subscribes to three additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R>(P, Q, R) -> Publishers.CombineLatest4&lt;Self, P, Q, R>

Subscribes to three additional publishers and publishes a tuple upon receiving output from any of the publishers.

