

- SpriteKit
-  SKAudioNode 

Class

# SKAudioNode

A node that plays audio.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKAudioNode
```

**watchOS**

``` source
class SKAudioNode
```

## Mentioned in 

Using Audio Nodes with the Scene’s Listener

## Overview

A SKAudioNode object is used to add an audio to a scene. The sounds are played automatically using AVFoundation, and the node can optionally add 3D spatial audio effects to the audio when it is played.

The currently presented SKScene object mixes the audio from nodes in the scene based on parameters defined in the AVAudio3DMixing protocol. A scene’s audioEngine property allows overall control of volume and playback.

By default, SKAudioNode objects are positional, i.e. their isPositional property is set to true. If you add an audio node to a scene with a listener set, SpriteKit will set the stereo balance and the volume based on the relative positions of the two nodes.

You can explicitly set the volume or stereo balance to an audio node by running actions on it.

SpriteKit includes actions that reduce an audio node’s volume by changing either its occlusion or obstruction. The difference between these actions is that occlusion affects both the direct and reverb paths of the sound while obstruction only affects the direct path. The *change volume* action offers absolute control over an audio node’s volume.

You can manually set the stereo balance of an audio node with a *stereo pan* action.

Special effects, such as speeding up or slowing down audio by changing the playback rate and adding reverb are also available as audio actions.

To learn more about audio actions, see Controlling the Audio of a Node in Action Initializers.

## Topics

### First Steps

Using Audio Nodes with the Scene’s Listener

Add audio to your scene, and optionally give it 2D-positional mixing characteristics.

### Initializing Audio Nodes

init(avAudioNode: AVAudioNode?)

Initializes an audio node from an AVFoundation audio node.

convenience init(fileNamed: String)

Initializes an audio node from an audio asset with the specified filename.

convenience init(url: URL)

Initializes an audio node from an audio asset with the specified URL.

init?(coder: NSCoder)

Tells you when to initialize an audio node that has been unarchived.

### Configuring Audio Nodes

var avAudioNode: AVAudioNode?

The audio node’s current audio asset.

var isPositional: Bool

A Boolean property that indicates whether the node’s audio is altered based on the position of the node.

var autoplayLooped: Bool

A Boolean value that indicates whether the audio should play in a loop when the node is added to the scene.

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Nodes for Environmental Effects

class SKLightNode

A node that lights surrounding nodes.

class SKFieldNode

A node that applies physics effects to nearby nodes.

