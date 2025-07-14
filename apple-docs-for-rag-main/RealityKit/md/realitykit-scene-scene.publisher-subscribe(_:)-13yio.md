

- RealityKit
- Scene
- Scene.Publisher
-  subscribe(\_:) 

Instance Method

# subscribe(\_:)

Attaches the specified subscriber to this publisher.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func subscribe(_ subscriber: S) where S : Subscriber, Self.Failure == S.Failure, Self.Output == S.Input
```

## Parameters 

`subscriber`  

The subscriber to attach to this publisher. After attaching, the subscriber can start to receive values.

## Discussion

Always call this function instead of receive(subscriber:). Adopters of Scene.Publisher must implement receive(subscriber:). The implementation of `Publisher/subscribe(_:)-4u8kn` provided by Scene.Publisher calls through to receive(subscriber:).

## See Also

### Working with subscribers

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

