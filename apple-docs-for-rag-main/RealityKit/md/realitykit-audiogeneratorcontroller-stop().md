

- RealityKit
- AudioGeneratorController
-  stop() 

Instance Method

# stop()

Stops playback of the render handler.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func stop()
```

## Discussion

Callbacks to the render handler stop after calling stop(). There may be a short delay between when you call `stop` and when the callbacks actually stop.

