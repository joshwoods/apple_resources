

- SceneKit
- Animation
-  Animating SceneKit Content 

Article

# Animating SceneKit Content

Learn about implicit animations, explicit animations, and actions, and when to choose each in your app.

## Overview

SceneKit animation support is based on the Core Animation framework. (For more about Core Animation, read Core Animation Programming Guide.) Several SceneKit classes define *animatable* properties, meaning that in addition to simply assigning a new value to the property, you can create animations that transition smoothly between two values of the property. For example, animating a node’s opacity property fades the node’s visible content in or out. You can animate content *implicitly* or *explicitly*.

### Animate Content Changes Implicitly

You create an animation implicitly by changing the value of an animatable property. Implicit animation is useful when you want to quickly animate a one-time change or animate several property changes together without writing a lot of animation code.

The SCNTransaction class defines SceneKit’s architecture for scene content changes, including implicit animations: A transaction is a single atomic operation that combines multiple changes to nodes, geometries, materials, or other scene content. By default, SceneKit automatically creates a default transaction for all changes you make to a scene during one pass through the run loop.

The default transaction’s duration is zero, so the changes you make to animatable properties occur immediately. However, if you increase the transaction’s animationDuration, all changes to animatable properties automatically animate. For example, changing the animation duration in an `IBAction` method causes both the position and opacity changes in that method to animate together.

Listing 1. Implicit animation that makes a block of text fall out of the scene while fading away

- Swift
- Objective-C

```
```

```
```

### Explicitly Create an Animation

For more complex animations, you can explicitly create an animation object and attach it to the scene element being animated. Creating an animation object also makes an animation reusable, so you can play the same animation at any time on demand or apply it to different elements of your scene.

Choose a CAAnimation subclass for the type of animation you want to create, specify the property to be animated using key-value coding, and set animation parameters. You then set the animation in motion by attaching it to one or more elements of your scene, as shown in Animating SceneKit Content.

By using different Core Animation classes, you can combine or sequence several animations or create animations that interpolate a property’s value between several keyframe values. For more about creating animation objects, see Core Animation Programming Guide. For more about attaching animations to SceneKit objects, see SCNAnimatable.

Listing 2. Explicit animation to vary the 3D extrusion depth of a block of text

- Swift
- Objective-C

```
```

```
```

SceneKit also uses CAAnimation objects for animations created using external 3D authoring tools and saved in scene files. For example, an artist might create a game character with animations for walking, jumping, and other actions. You incorporate these animations into your game by loading animation objects from the scene file using the SCNSceneSource class and attaching them to the SCNNode object that represents the game character.

