

- RealityKit
-  AnimationEvents 

Enumeration

# AnimationEvents

Notable milestones that the framework signals during animation playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
enum AnimationEvents
```

## Overview

This enumeration defines the playback states that an animated entity can indicate to an app. To receive notification of a particular event, create a completion handler:

```
private func onAnimationCompleted(_ event:
    AnimationEvents.PlaybackCompleted) {
        // Define code that runs when the animation completes.
}
```

Then, subscribe the handler on the entity for the state of interest:

```
// Get an animation.
let animationName =
entity.availableAnimations.first!.name!

// Pass the animation to an entity and get a controller.
entity.playAnimation(named: animationName, transitionDuration: 0.0)

entitySubscription = view.scene.publisher(for:
    AnimationEvents.PlaybackCompleted.self, on: entity)
        .sink(receiveValue: onAnimationCompleted)
```

## Topics

### Recognizing animation events

struct PlaybackStarted

The event raised when an animation has been started.

struct PlaybackCompleted

The event raised when an animation reaches the end of its duration.

struct PlaybackLooped

The event raised when an animation loops.

struct PlaybackTerminated

The event raised when an animation has been terminated, regardless of whether it ran to completion.

### Recognizing skeletal events

struct SkeletalPoseUpdateComplete

Raised immediately after the SkeletalPoseSystem has been updated.

## See Also

### Physics and motion events

enum CollisionEvents

enum PhysicsSimulationEvents

Types of events that fire during physics simulations

