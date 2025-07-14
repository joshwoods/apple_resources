

- SceneKit
- SCNSceneRenderer
-  audioEnvironmentNode 

Instance Property

# audioEnvironmentNode

The 3D audio mixing node SceneKit uses for positional audio effects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var audioEnvironmentNode: AVAudioEnvironmentNode { get }
```

**Required**

## Discussion

SceneKit uses this audio node to spatialize sounds from SCNAudioPlayer objects attached to nodes in the scene. You can use this object in conjunction with the audioEngine property to rearrange the audio graph to add other, non-spatialized audio sources or mix in audio processing effects.

## See Also

### Working With Positional Audio

var audioListener: SCNNode?

The node representing the listener’s position in the scene for use with positional audio effects.

**Required**

var audioEngine: AVAudioEngine

The audio engine SceneKit uses for playing scene sounds.

**Required**

