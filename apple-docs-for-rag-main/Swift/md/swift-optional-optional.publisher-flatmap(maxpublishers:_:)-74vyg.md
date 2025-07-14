

- Swift
- Optional
- Optional.Publisher
-  flatMap(maxPublishers:\_:) 

Instance Method

# flatMap(maxPublishers:\_:)

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

SwiftCombineiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func flatMap(
    maxPublishers: Subscribers.Demand = .unlimited,
    _ transform: @escaping (Self.Output) -> P
) -> Publishers.FlatMap, Self> where P : Publisher, P.Failure == Never
```

## Parameters 

`maxPublishers`  

Specifies the maximum number of concurrent publisher subscriptions, or `Combine/Subscribers/Demand/unlimited` if unspecified.

`transform`  

A closure that takes an element as a parameter and returns a publisher that produces elements of that type.

## Return Value

A publisher that transforms elements from an upstream publisher into a publisher of that element’s type.

