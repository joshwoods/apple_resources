

- PHASE
-  Sound Event Nodes 

API Collection

# Sound Event Nodes

Objects that connect to form a hierarchical tree of audio actions.

## Overview

To play sound, your app assembles a hieararchical structure of audio *nodes* that determine which sound to play at the moment. A tree with two sampler nodes branching from a switch node plays only one sampler, depending on your app’s state. You set the control logic in advance that specifies the conditions upon which the switch node toggles. To play the same audio consistently, create a tree with a single sampler node.

To invoke the tree, create a sound event that references the tree and call start(completion:) on the sound event.

## Topics

### Audio-Providing Nodes

class PHASESamplerNodeDefinition

A node that plays complete audio data.

enum PHASEPlaybackMode

Loop options for audio playback.

class PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

class PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

struct PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

enum PHASECalibrationMode

Calibration options for sound pressure level.

class PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

### Control Nodes

class PHASESwitchNodeDefinition

A node that passes invocation to only one of its child nodes.

class PHASERandomNodeDefinition

A sound event node that invokes one of its child nodes at random.

class PHASEBlendNodeDefinition

A node that smoothly fades between the audio of its child nodes.

class PHASEContainerNodeDefinition

A node that plays all its children at the same time.

## See Also

### Audio Selection and Playback

class PHASESoundAsset

A sound resource stored in the asset registry.

class PHASESoundEvent

An object that determines which audio to play.

enum RenderingState

The playback status of audio.

class PHASESoundEventNodeDefinition

A base class for sound event nodes that connect to form a node hierarchy.

class PHASESoundEventNodeAsset

A template object for sounds that can play in reaction to environmental state.

class PHASEAsset

A base class that adds a name to framework assets.

