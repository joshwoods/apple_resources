

- RealityKit
-  AnimationPlaybackController 

Class

# AnimationPlaybackController

A controller that manages animation playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class AnimationPlaybackController
```

## Overview

This class controls the playback of an entity animation by providing its pause, resume, or stop functions.

The animation starts immediately after you call playAnimation(_:transitionDuration:startsPaused:), or move(to:relativeTo:duration:timingFunction:), which both return an instance of this class.

A controller invalidates after its associated animation completes or stops. To play another animation, perform an action that generates another controller.

While an animation plays, you can receive notification of particular playback states by subscribing to an event. For more information, see AnimationEvents.

## Topics

### Inspecting and controlling playback

func pause()

Pauses the animation.

func resume()

Resumes a paused animation.

func stop()

Stops an animation.

var isPlaying: Bool

A Boolean value that indicates whether the animation plays.

var isStopped: Bool

A Boolean value that indicates whether the animation stopped.

var isValid: Bool

A Boolean value that indicates whether the animation controller is functional.

var blendFactor: Float

The level of influence the controller gives to its animation.

### Managing completion

var isComplete: Bool

A Boolean that indicates whether the animation has finished running.

var isPaused: Bool

A Boolean that indicates whether the animation is paused.

### Accessing the associated entity

var entity: Entity?

The entity to which the animation applies.

### Timing animation playback

var duration: TimeInterval

The length of time the animation spans, in seconds.

var speed: Float

The animation’s rate of playback.

var clock: CMClockOrTimebase

A reference clock to synchronize the animation with other events.

var time: TimeInterval

The animation’s location within the timeline.

### Comparing animation playback controllers

static func == (AnimationPlaybackController, AnimationPlaybackController) -> Bool

Indicates whether two animation playback controllers are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the controller by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Instance Methods

func stop(blendOutDuration: TimeInterval)

Stops an animation with a fade-out time.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Animation playback

class AnimationResource

An animation for the properties of scenes or entities.

struct AnimationLibraryComponent

A component that represents a collection of animations that an entity can play.

struct AnimationCollection

A collection of animations an entity can play.

enum AnimationEvents

Notable milestones that the framework signals during animation playback.

enum AnimationRepeatMode

Options that determine whether an animation replays after completion.

