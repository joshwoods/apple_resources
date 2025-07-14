

- RealityKit
-  AnimationLibraryComponent 

Structure

# AnimationLibraryComponent

A component that represents a collection of animations that an entity can play.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct AnimationLibraryComponent
```

## Overview

You use an `AnimationLibraryComponent` to access an entity’s animation resources. You can store animations with an entity by packaging them together into a `.reality` file. You can do this with Reality Composer Pro or by building a custom tool.

### Create an animation library with Reality Composer Pro

Follow these steps to create an animation library for an entity:

1.  In the hierarchy view, select the entity you want to add animations to.

2.  In the inspector, click Add Component and select Animation Library from the list of components.

3.  Click the Add button (+) and select the USD files with animations.

Tip

See Designing RealityKit content with Reality Composer Pro for more details on working with components in Reality Composer Pro.

At runtime, your app can access and play the animations that the entity stores.

```
// Load the entity you want to animate.
let robot = try await Entity(named: "robot")

// Access the animation library associated with the entity.
let animationLibrary = robot.components[AnimationLibraryComponent.self]

// Play the walk animation.
if let walkAnimation = animationLibrary.animations["walk"] {
    robot.playAnimation(walkAnimation)
}
```

### Create an animation library by building your own tool

If you need to build a custom tool to create `.reality` files, you can use RealityKit to programmatically create an animation library by following these steps:

1.  Load an animation entity with init(named:in:).

2.  Retrieve the entity’s animation resources from its availableAnimations property.

3.  Add the animations to an animation library.

The following example shows how you can set up an animation library:

```
// Create an empty animation library component.
var animationLibrary = AnimationLibraryComponent()

// Load the entities containing the animations.
let entityIdleAnimation = try await Entity(named: "idle")
let entityWalkAnimation = try await Entity(named: "walk")

// Assign the animations to the library by name.
animationLibrary.animations["idle"] = entityIdleAnimation.availableAnimations.first
animationLibrary.animations["walk"] = entityWalkAnimation.availableAnimations.first
```

After you configure the animation library, you can assign it to an entity and serialize the entity to a file. RealityKit packages the animations for that entity when you save it to a `.reality` file.

```
// Load the entity you want to animate.
let robot = try! await Entity(named: "robot")

// Assign the animation library to the entity.
robot.components.set(animationLibrary)

// Write the entity with its animations to a file.
robot.write(to: fileURL)
```

To play one of the animations in your app, create an entity from the `.reality` file and then call its playAnimation(_:transitionDuration:startsPaused:) method.

## Topics

### Creating an animation library component

init()

Creates an empty animation library.

init(animations: [String : AnimationResource])

Creates an animation library from a dictionary that associates an animation’s data with its name.

init(dictionaryLiteral: (String, AnimationResource)...)

Creates an animation library from a variadic list of key-value pairs.

### Accessing animations

var animations: AnimationLibraryComponent.AnimationCollection

The collection of animations an entity can play.

var unkeyedResources: [AnimationResource]?

The library’s animation resources that don’t have a queryable name.

var defaultAnimation: AnimationResource?

The default animation resource.

var defaultKey: String?

The name of the default animation resource.

### Managing references to animations

func removeAll(resource: AnimationResource)

Removes all the component’s references to an animation resource.

### Structures

struct AnimationCollection

A collection of animations an entity can play.

### Type Aliases

typealias Key

The key type of a dictionary literal.

typealias Value

The value type of a dictionary literal.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component
- ExpressibleByDictionaryLiteral

## See Also

### Animation playback

class AnimationResource

An animation for the properties of scenes or entities.

struct AnimationCollection

A collection of animations an entity can play.

enum AnimationEvents

Notable milestones that the framework signals during animation playback.

class AnimationPlaybackController

A controller that manages animation playback.

enum AnimationRepeatMode

Options that determine whether an animation replays after completion.

