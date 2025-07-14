

- SpriteKit
- SKAudioNode
-  avAudioNode 

Instance Property

# avAudioNode

The audio node’s current audio asset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var avAudioNode: AVAudioNode? { get set }
```

**watchOS**

``` source
var avAudioNode: AVAudioNode? { get set }
```

## Discussion

The AV audio node must refer to an AVAudioEngine sound graph from a single sound source or URL.

## See Also

### Configuring Audio Nodes

var isPositional: Bool

A Boolean property that indicates whether the node’s audio is altered based on the position of the node.

var autoplayLooped: Bool

A Boolean value that indicates whether the audio should play in a loop when the node is added to the scene.

