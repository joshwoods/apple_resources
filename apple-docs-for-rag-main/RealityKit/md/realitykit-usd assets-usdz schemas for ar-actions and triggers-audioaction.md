

- RealityKit
- USD Assets
- USDZ schemas for AR
- Actions and triggers
-  AudioAction 

# AudioAction

An action that plays audio.

## Overview

This prim implements one of two ways to play audio in a scene; to play audio without AudioAction, use SpatialAudio.

### Declaration

```
class Preliminary_Action "AudioAction"
```

## Topics

### Properties

info:id

The action’s unique identifier.

affectedObjects

A list of prims that respond to the notification.

audio

The location of an audio file.

type

An option that controls the order in which the actions execute.

gain

A value that controls the audio volume.

auralMode

An option that controls the audio signal’s spacial dynamics.

## See Also

### Actions

Preliminary_Action

A specific task that a trigger performs.

ChangeSceneAction

An action that transitions from one scene to another.

EmphasizeAction

An action that performs an animation to call attention to an object.

GroupAction

An action that runs a list of other actions.

ImpulseAction

An action that adds velocity to an prim.

LookAtCameraAction

An action that reorients an object to face the user’s camera.

OrbitAction

An action that orbits a set of prims around another.

SpinAction

An action that spins a prim.

StartAnimationAction

An action that plays an asset’s animation.

TransformAction

An action that animates from one transform to another.

TransformAnimationAction

An action that plays a transform animation.

VisibilityAction

An action that displays or hides objects over a period of time.

WaitAction

An action that performs a delay.

NotificationAction

An action that sends a custom notification to an app.

