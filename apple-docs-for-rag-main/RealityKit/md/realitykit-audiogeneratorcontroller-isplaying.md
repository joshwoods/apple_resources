

- RealityKit
- AudioGeneratorController
-  isPlaying 

Instance Property

# isPlaying

A Boolean value that indicates whether playback is currently active.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
var isPlaying: Bool { get }
```

## Discussion

You may experience a small delay between when you call the play() method and when the isPlaying property reports `true`.

