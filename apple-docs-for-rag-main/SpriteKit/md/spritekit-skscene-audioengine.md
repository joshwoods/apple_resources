

- SpriteKit
- SKScene
-  audioEngine 

Instance Property

# audioEngine

The AVFoundation audio engine used to play audio from audio nodes contained in the scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var audioEngine: AVAudioEngine { get }
```

**watchOS**

``` source
var audioEngine: AVAudioEngine { get }
```

## Discussion

An audio engine instance is automatically created for you when the scene is created. You can use methods and properties on a scene’s audio engine for overall control of all of its child audio nodes. The following code shows how a scene’s overall volume can be reduced from its default of 1.0 down to 0.2 and then paused:

```
let scene = SKScene()
scene.audioEngine.mainMixerNode.outputVolume = 0.2
scene.audioEngine.pause()
```

## See Also

### Adding Positional Audio

Using Audio Nodes with the Scene’s Listener

Add audio to your scene, and optionally give it 2D-positional mixing characteristics.

var listener: SKNode?

A node used to determine the position of the listener for positional audio in the scene.

