

- Combine
- Publishers
- Publishers.MeasureInterval
-  flatMap(maxPublishers:\_:) 

Instance Method

# flatMap(maxPublishers:\_:)

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func flatMap(
    maxPublishers: Subscribers.Demand = .unlimited,
    _ transform: @escaping (Self.Output) -> P
) -> Publishers.FlatMap where T == P.Output, P : Publisher, Self.Failure == P.Failure
```

## Parameters 

`maxPublishers`  

Specifies the maximum number of concurrent publisher subscriptions, or unlimited if unspecified.

`transform`  

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

## Return Value

A publisher that transforms elements from an upstream publisher into a publisher of that element’s type.

## Discussion

Combine‘s `flatMap(maxPublishers:_:)` operator performs a similar function to the flatMap(_:) operator in the Swift standard library, but turns the elements from one kind of publisher into a new publisher that is sent to subscribers. Use `flatMap(maxPublishers:_:)` when you want to create a new series of events for downstream subscribers based on the received value. The closure creates the new Publisher based on the received value. The new Publisher can emit more than one event, and successful completion of the new Publisher does not complete the overall stream. Failure of the new Publisher causes the overall stream to fail.

In the example below, a PassthroughSubject publishes `WeatherStation` elements. The `flatMap(maxPublishers:_:)` receives each element, creates a URL from it, and produces a new URLSession.DataTaskPublisher, which will publish the data loaded from that URL.

```
public struct WeatherStation {
    public let stationID: String
}

var weatherPublisher = PassthroughSubject()

cancellable = weatherPublisher.flatMap { station -> URLSession.DataTaskPublisher in
    let url = URL(string:"https://weatherapi.example.com/stations/\(station.stationID)/observations/latest")!
    return URLSession.shared.dataTaskPublisher(for: url)
}
.sink(
    receiveCompletion: { completion in
        // Handle publisher completion (normal or error).
    },
    receiveValue: {
        // Process the received data.
    }
 )

weatherPublisher.send(WeatherStation(stationID: "KSFO")) // San Francisco, CA
weatherPublisher.send(WeatherStation(stationID: "EGLC")) // London, UK
weatherPublisher.send(WeatherStation(stationID: "ZBBB")) // Beijing, CN
```

## See Also

### Republishing Elements by Subscribing to New Publishers

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Publishers.SetFailureType&lt;Self, P.Failure>>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;Publishers.SetFailureType&lt;P, Self.Failure>, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func switchToLatest() -> Publishers.SwitchToLatest&lt;Self.Output, Publishers.SetFailureType&lt;Self, Self.Output.Failure>>

Republishes elements sent by the most recently received publisher.

