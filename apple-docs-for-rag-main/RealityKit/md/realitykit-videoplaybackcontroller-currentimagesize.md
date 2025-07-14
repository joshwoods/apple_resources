

- RealityKit
- VideoPlaybackController
-  currentImageSize 

Instance Property

# currentImageSize

What is the width and height of currently playing video (for stereo, the width and height of each eye)? This is optional because the video may not currently be playing, or the size is otherwise not available.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
var currentImageSize: CGSize? { get }
```

