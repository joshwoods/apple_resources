

- RealityKit
- AudioPlaybackController
-  completionHandler 

Instance Property

# completionHandler

A closure that the playback controller executes when it reaches the end of the audio stream.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var completionHandler: (() -> Void)? { get set }
```

## Discussion

The controller doesn’t call the closure if you manually stop the audio by calling the stop() or the pause() method.

Note

You can only register one handler at a time. If you set a new handler, the controller discards the old one.

