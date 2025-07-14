

- RealityKit
-  PlayAudioAction 

Structure

# PlayAudioAction

An action which plays an audio resource on the given target entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct PlayAudioAction
```

## Overview

Use this action to initiate the playback of audio in a data-driven way. For example, this action can play an animation group which contains a nested action, which plays audio with specific playback properties.

This action plays the AudioResource from the AudioLibraryComponent on the targetEntity. Add all audio resources to the audio library component that this action will play, ensuring the name of the audio matches the audioResourceName being supplied.

useControlledPlayback is used to determine the playback behavior of the audio this action is playing. Set this to `true` to control the playback of the audio. Calling methods such as pause() and resume() on the animation playback controller generated from this action will give you control of the audio being played. When the action ends, the audio playback also ends. Set this to `false` to ensure the audio being played runs independently of the action. This would behave as a one shot audio.

The example below creates an animation which will play an audio resource after five seconds.

```
// Create an action which plays a specified audio resource.
//
// The audio resource exists within the target entity's
// animation library component.
//
// Control playback is set to false, audio will
// play independently of the animation.
let snapAudioAction = PlayAudioAction(audioResourceName: "snap",
                                      useControlledPlayback: false)

// Creates an animation from the action, with a five second delay.
let snapAudioAnimation = try AnimationResource
    .makeActionAnimation(for: snapAudioAction,
                         delay: 5.0)

// Play the animation which will play the audio after five seconds.
entity.playAnimation(snapAudioAnimation)
```

Note

If useControlledPlayback is set to `true`, the animation will play for the duration of the action. Set the duration of the action to match the length of the audio being played to ensure the entire audio plays.

Important

This action does not directly animate a bound property, such as BindTarget.transform.

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(targetEntity: ActionEntityResolution, audioResourceName: String, gain: Audio.Decibel, useControlledPlayback: Bool)

Creates a new play audio action.

### Instance Properties

var animatedValueType: (any AnimatableData.Type)?

The type for the value that the action modifies over time.

var audioResourceName: String

The name of the audio stored in audio library component of the target entity to start playing.

var gain: Audio.Decibel

The individual gain in decibels of the audio.

var targetEntity: ActionEntityResolution

The entity to play the audio.

var useControlledPlayback: Bool

A Boolean that indicates whether this action has control over the playback of the audio.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Aliases

typealias EventParameterType

The associated event parameter type.

### Default Implementations

EntityAction Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- EntityAction

## See Also

### Built-in actions

struct BillboardAction

An action that animates the blend factor of an entity’s billboard component.

struct EmphasizeAction

An action that performs an animation to call attention to an entity.

struct FromToByAction

An action that starts, stops, or increments by a specific value.

struct ImpulseAction

An action that applies an impulse to the physics body at its center of mass when played as an animation.

struct OrbitEntityAction

An action which animates the transform of an entity to revolve around a specified pivot entity.

struct PlayAnimationAction

An action that plays an animation on the given target entity with a range of playback options.

struct SetEntityEnabledAction

An action that enables or disables the targeted entity and its descendants when played as an animation.

struct SpinAction

An action which animates the transform of an entity to rotate around a specified local axis.

