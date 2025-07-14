

- RealityKit
-  Entity animations 

API Collection

# Entity animations

Dynamically move, rotate, and scale entities at runtime.

## Topics

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

enum AnimationRepeatMode

Options that determine whether an animation replays after completion.

### Animation definitions

struct SampledAnimation

An animation that cycles through a series of frames at a constant interval.

enum TweenMode

Options that determine whether an animation switches between frames gradually or abruptly.

struct FromToByAnimation

An animation that starts, stops, or increments by a specific value.

struct AnimationTimingFunction

The pacing of an animation transition.

struct AnimationView

An animation that represents a variation of another animation.

struct OrbitAnimation

An animation that revolves an entity around its origin.

protocol AnimationDefinition

The configuration, including target object, timeframe, and visual semantics, of an animation.

struct AnimationFillMode

Options that determine which animation frames display outside of the normal duration.

struct AnimationGroup

A collection of animations that play simultaneously.

struct AnimationHandoffType

The type of handoff the play animation method performs between a current animation and a new animation.

### Bindable animation targets

struct BindPath

The components of a target’s path that refer to the animation properties of a nested scene or entity.

enum BindTarget

A reference to a particular scene, entity, or property that animates.

struct BindableValue

The value of a bindable target.

struct BindableValuesReference

A reference to a bindable value of an animation.

struct ParameterSet

A reference to general-purpose entity parameters for animations.

struct InternalBindPath

A bind target for framework-provided properties.

### Compliance-related protocols

protocol AnimatableData

A functionality specification that animatable data types adopt.

protocol BindableData

An opaque base protocol for bindable data objects.

### Blend trees

struct BlendTreeAnimation

A collection of animations on the same property that the framework blends to a single animation.

protocol BlendTreeNode

An interface for a node that’s a member of a blend tree.

struct BlendTreeBlendNode

A source node for an animation that mixes several animations to form a single animation.

struct BlendTreeSourceNode

A blend node that contains an animation.

struct BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

enum BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

## See Also

### Game development

Gaming sample code projects

Explore a collection of projects relating to game development.

Character control, skeletons, and inverse kinematics

Direct the movements and animation of models.

