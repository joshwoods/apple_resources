

- SpriteKit
- SKAudioNode
-  isPositional 

Instance Property

# isPositional

A Boolean property that indicates whether the node’s audio is altered based on the position of the node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isPositional: Bool { get set }
```

**watchOS**

``` source
var isPositional: Bool { get set }
```

## Discussion

If true, the audio mixer considers the position and velocity of the SKAudioNode relative to scene’s current listener node. The mixer applies distance attenuation, doppler shift, and pan effects to the sound. If false, then the sound is played normally. The default value is true.

## See Also

### Configuring Audio Nodes

var avAudioNode: AVAudioNode?

The audio node’s current audio asset.

var autoplayLooped: Bool

A Boolean value that indicates whether the audio should play in a loop when the node is added to the scene.

