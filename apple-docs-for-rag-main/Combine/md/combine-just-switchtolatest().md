

- Combine
- Just
-  switchToLatest() 

Instance Method

# switchToLatest()

Republishes elements sent by the most recently received publisher.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func switchToLatest() -> Publishers.SwitchToLatest>
```

Available when `Failure` is `Never` and `Output` conforms to `Publisher`.

## Discussion

This operator works with an upstream publisher of publishers, flattening the stream of elements to appear as if they were coming from a single stream of elements. It switches the inner publisher as new ones arrive but keeps the outer publisher constant for downstream subscribers.

When this operator receives a new publisher from the upstream publisher, it cancels its previous subscription. Use this feature to prevent earlier publishers from performing unnecessary work, such as creating network request publishers from frequently updating user interface publishers.

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

