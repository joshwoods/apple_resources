

- RealityKit
- Scene
- Scene.Publisher
-  receive(subscriber:) 

Instance Method

# receive(subscriber:)

Attaches the specified subscriber to this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
func receive(subscriber: S) where E == S.Input, S : Subscriber, S.Failure == Never
```

## Parameters 

`subscriber`  

The subscriber to attach to this Scene.Publisher, after which it can receive values.

## Discussion

Implementations of Scene.Publisher must implement this method.

The provided implementation of `Publisher/subscribe(_:)-4u8kn`calls this method.

## See Also

### Working with subscribers

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

