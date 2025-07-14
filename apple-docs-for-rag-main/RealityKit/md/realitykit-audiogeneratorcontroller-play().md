

- RealityKit
- AudioGeneratorController
-  play() 

Instance Method

# play()

Begins the audio stream from the generator render handler.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func play()
```

## Discussion

When you play the controller, the render handler starts receiving callbacks. The controller ignores calls to play() when audio is already playing.

