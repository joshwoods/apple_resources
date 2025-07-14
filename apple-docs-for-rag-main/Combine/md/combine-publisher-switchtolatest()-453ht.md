

- Combine
- Publisher
-  switchToLatest() 

Instance Method

# switchToLatest()

Republishes elements sent by the most recently received publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func switchToLatest() -> Publishers.SwitchToLatest
```

Available when `Failure` is `Self.Output.Failure` and `Output` conforms to `Publisher`.

## Discussion

This operator works with an upstream publisher of publishers, flattening the stream of elements to appear as if they were coming from a single stream of elements. It switches the inner publisher as new ones arrive but keeps the outer publisher constant for downstream subscribers.

For example, given the type `AnyPublisher`, calling `switchToLatest()` results in the type `SwitchToLatest`. The downstream subscriber sees a continuous stream of `(Data, URLResponse)` elements from what looks like a single URLSession.DataTaskPublisher even though the elements are coming from different upstream publishers.

When this operator receives a new publisher from the upstream publisher, it cancels its previous subscription. Use this feature to prevent earlier publishers from performing unnecessary work, such as creating network request publishers from frequently updating user interface publishers.

The following example updates a PassthroughSubject with a new value every `0.1` seconds. A map(_:) operator receives the new value and uses it to create a new URLSession.DataTaskPublisher. By using the `switchToLatest()` operator, the downstream sink subscriber receives the `(Data, URLResponse)` output type from the data task publishers, rather than the URLSession.DataTaskPublisher type produced by the map(_:) operator. Furthermore, creating each new data task publisher cancels the previous data task publisher.

```
let subject = PassthroughSubject()
cancellable = subject
    .setFailureType(to: URLError.self)
    .map() { index -> URLSession.DataTaskPublisher in
        let url = URL(string: "https://example.org/get?index=\(index)")!
        return URLSession.shared.dataTaskPublisher(for: url)
    }
    .switchToLatest()
    .sink(receiveCompletion: { print("Complete: \($0)") },
          receiveValue: { (data, response) in
            guard let url = response.url else { print("Bad response."); return }
            print("URL: \(url)")
    })

for index in 1...5 {
    DispatchQueue.main.asyncAfter(deadline: .now() + TimeInterval(index/10)) {
        subject.send(index)
    }
}

// Prints "URL: https://example.org/get?index=5"
```

The exact behavior of this example depends on the value of `asyncAfter` and the speed of the network connection. If the delay value is longer, or the network connection is fast, the earlier data tasks may complete before `switchToLatest()` can cancel them. If this happens, the output includes multiple URLs whose tasks complete before cancellation.

## See Also

### Republishing Elements by Subscribing to New Publishers

func flatMap&lt;T, P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Publishers.SetFailureType&lt;Self, P.Failure>>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;Publishers.SetFailureType&lt;P, Self.Failure>, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func switchToLatest() -> Publishers.SwitchToLatest&lt;Self.Output, Publishers.SetFailureType&lt;Self, Self.Output.Failure>>

Republishes elements sent by the most recently received publisher.

func switchToLatest() -> Publishers.SwitchToLatest&lt;Publishers.SetFailureType&lt;Self.Output, Self.Failure>, Publishers.Map&lt;Self, Publishers.SetFailureType&lt;Self.Output, Self.Failure>>>

Republishes elements sent by the most recently received publisher.

func switchToLatest() -> Publishers.SwitchToLatest&lt;Self.Output, Self>

Republishes elements sent by the most recently received publisher.

