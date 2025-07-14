

- RealityKit
- Scene
- Scene.Publisher
-  switchToLatest() 

Instance Method

# switchToLatest()

Republishes elements sent by the most recently received publisher.

RealityKitCombineiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func switchToLatest() -> Publishers.SwitchToLatest>
```

Available when `Failure` is `Never` and `Output` conforms to `Publisher`.

## Discussion

This operator works with an upstream publisher of publishers, flattening the stream of elements to appear as if they were coming from a single stream of elements. It switches the inner publisher as new ones arrive but keeps the outer publisher constant for downstream subscribers.

When this operator receives a new publisher from the upstream publisher, it cancels its previous subscription. Use this feature to prevent earlier publishers from performing unnecessary work, such as creating network request publishers from frequently updating user interface publishers.

