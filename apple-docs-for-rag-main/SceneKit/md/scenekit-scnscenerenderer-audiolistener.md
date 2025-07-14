

- SceneKit
- SCNSceneRenderer
-  audioListener 

Instance Property

# audioListener

The node representing the listener’s position in the scene for use with positional audio effects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var audioListener: SCNNode? { get set }
```

**Required**

## Discussion

When you use the SCNAudioPlayer class to play sound, the resulting effect depends on the position of each audio source in the scene relative to the listener. For example, changes in relative position can cause a sound to be localized to the left or right channel for stereo headphone output.

This property determines the listener’s position. If the value is `nil` (the default), the listener position is always the same as that of the pointOfView node. By providing a different node for this property, you can separate the listener position from the point of view—this produces an effect similar to that of a boom microphone in video production. For example, in a third-person game where the camera floats high in the sky above the player character, you might use the player character as the listener node so that sounds from positions nearest the player are loudest.

To place an audio source in the scene, use the addAudioPlayer(_:) method on an SCNNode object.

## See Also

### Working With Positional Audio

var audioEnvironmentNode: AVAudioEnvironmentNode

The 3D audio mixing node SceneKit uses for positional audio effects.

**Required**

var audioEngine: AVAudioEngine

The audio engine SceneKit uses for playing scene sounds.

**Required**

