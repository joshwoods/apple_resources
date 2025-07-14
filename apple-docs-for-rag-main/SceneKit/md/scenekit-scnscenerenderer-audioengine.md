

- SceneKit
- SCNSceneRenderer
-  audioEngine 

Instance Property

# audioEngine

The audio engine SceneKit uses for playing scene sounds.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var audioEngine: AVAudioEngine { get }
```

**Required**

## Discussion

SceneKit uses this audio engine to play sounds from SCNAudioPlayer objects attached to nodes in the scene. You can use this object directly to add other sound sources not related to scene contents, or to add other sound processing nodes or mixing nodes to the audio engine. To identify the node SceneKit uses for spatializing scene sounds when connecting other nodes, use the audioEnvironmentNode property.

## See Also

### Working With Positional Audio

var audioListener: SCNNode?

The node representing the listener’s position in the scene for use with positional audio effects.

**Required**

var audioEnvironmentNode: AVAudioEnvironmentNode

The 3D audio mixing node SceneKit uses for positional audio effects.

**Required**

