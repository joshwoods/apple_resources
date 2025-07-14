

- RealityKit
-  AnimationRepeatMode 

Enumeration

# AnimationRepeatMode

Options that determine whether an animation replays after completion.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum AnimationRepeatMode
```

## Overview

Adopters of AnimationDefinition, such as SampledAnimation, offer repeat options of this type through the repeatMode property.

To select a behavior, set the repeat mode as you configure your animation, as in the following example:

```
let clip = FromToByAnimation()
clip.repeatMode = .repeat
```

## Topics

### Choosing a repeat mode

case `repeat`

A mode that restarts the animation after it completes.

case cumulative

A mode that repeats indefinitely and begins each repetition by setting the animated property to the ending value of the previous repetition.

case autoReverse

A mode that reverses the animation after reaching the end or the beginning.

case none

An option that determines the animation doesn’t repeat.

### Comparing repeat modes

static func == (AnimationRepeatMode, AnimationRepeatMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

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

class AnimationPlaybackController

A controller that manages animation playback.

