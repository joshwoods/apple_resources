

- RealityKit
- VideoMaterial
-  controller 

Instance Property

# controller

An object that configures framework-specific video options.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
var controller: VideoPlaybackController { get }
```

## Discussion

Use this property to configure AR-specific properties of the texture’s video, such as whether the material should use spatial audio.

The following example demonstrates enabling spatial audio for a video material:

```
material.controller.audioInputMode = .spatial
```

## See Also

### Controlling playback

var avPlayer: AVPlayer?

The material’s video playback controller.

