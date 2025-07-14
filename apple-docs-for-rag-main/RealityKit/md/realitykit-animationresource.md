

- RealityKit
-  AnimationResource 

Class

# AnimationResource

An animation for the properties of scenes or entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class AnimationResource
```

## Overview

You find animation resources in an entity’s availableAnimations array. Animation resources come bundled with an entity when you load the entity from a file. They describe an animation that’s specific to the entity to which they are attached.

Use the entity’s playAnimation(_:transitionDuration:startsPaused:) method to play a particular item in its animation resource array, or the `playAnimation(named:transitionDuration:startsPaused:)` method to play all of the animations with a given name. From both methods, you receive an AnimationPlaybackController instance that lets you manage playback of the resource.

If you want to loop an animation, call the resource’s repeat(count:) method to create a new resource that plays a given number of times in a row, or call the repeat(duration:) method to create a new resource that loops for the given duration. The latter loops indefinitely if you omit the duration parameter. You use the new animation resource that these methods return just as you would any other.

## Topics

### Creating an animation resource

static func generate(with: any AnimationDefinition) throws -> AnimationResource

Creates an animation resource from a definition.

static func sequence(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that plays a collection of animations in a specified sequence.

static func group(with: [AnimationResource]) throws -> AnimationResource

Creates an animation resource that simultaneously plays back a collection of animations.

func `repeat`(count: Int) -> AnimationResource

Creates an animation that repeats the specified number of times.

func `repeat`(duration: TimeInterval) -> AnimationResource

Repeats an animation for the specified amount of time.

### Inspecting animation information

let name: String?

The name of the animation resource.

var definition: any AnimationDefinition

The timeframe, target object, and visual semantics of the animation.

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

### Associating an animation with an entity

func store(in: Entity)

Adds the animation to an entity without playing it.

### Type Methods

static func makeActionAnimation&lt;T>(for: T, duration: TimeInterval, name: String, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float) throws -> AnimationResource

Creates an action animation containing a single event definition from an action.

## Relationships

### Conforms To

- Resource
- Sendable

## See Also

### Animation playback

struct AnimationLibraryComponent

A component that represents a collection of animations that an entity can play.

struct AnimationCollection

A collection of animations an entity can play.

enum AnimationEvents

Notable milestones that the framework signals during animation playback.

class AnimationPlaybackController

A controller that manages animation playback.

enum AnimationRepeatMode

Options that determine whether an animation replays after completion.

