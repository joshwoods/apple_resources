

- RealityKit
- VideoPlaybackController
-  currentViewingMode 

Instance Property

# currentViewingMode

Is the currently playing video in mono or stereo? This is optional because the video may not currently be playing, or the mode is otherwise not available.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
var currentViewingMode: VideoPlaybackController.ViewingMode? { get }
```

