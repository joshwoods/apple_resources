

- SpriteKit
- SKAction
-  Action Initializers 

API Collection

# Action Initializers

Use these functions to create actions.

## Overview

Most actions implement specific predefined animations that are done for you by SpriteKit. If your animation needs fall outside of the suite provided here, then you should:

- Consider using the methods in Creating Custom Actions below (never subclass `SKAction`)

- Consider the advice in Drive Game Logic

### Choose an Initializer for the Property You Want to Alter

Most actions allow you to change a node’s properties and some actions specifically apply to specific nodes, like SKSpriteNode’s actions for animating its color or texture.

Here are the most common animated properties:

- Changing a node’s position and zRotation

- Changing a node’s `size` or scaling properties

- Changing a node’s visibility or making it translucent

- Changing a sprite node’s contents so that it animates through a series of textures

- Colorizing a sprite node

- Playing sounds

- Removing a node from the node tree

- Calling a block

- Invoking a selector on an object

See Action Initializers for a full list of action types.

### Chaining Actions

Actions can be chained together in multiple ways:

- A *sequence action* has multiple child actions. Each action in the sequence begins after the previous action ends.

- A *group action* has multiple child actions. All actions stored in the group begin executing at the same time.

- A *repeating action* stores a single child action. When the child action completes, it is restarted.

To delay a subsequent action in the chain, insert a wait(forDuration:) action in the sequence, and remember that groups, sequences, and repeating actions may be nested.

## Topics

### Animating a Node’s Position in a Linear Path

Animate linear node movement.

class func moveBy(x: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node relative to its current position.

class func move(by: CGVector, duration: TimeInterval) -> SKAction

Creates an action that moves a node relative to its current position.

class func move(to: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that moves a node to a new position.

class func moveTo(x: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node horizontally.

class func moveTo(y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that moves a node vertically.

### Animating a Node’s Position Along a Custom Path

Provide a path for the node to follow.

class func follow(CGPath, duration: TimeInterval) -> SKAction

Creates an action that moves the node along a relative path, orienting the node to the path.

class func follow(CGPath, speed: CGFloat) -> SKAction

Creates an action that moves the node along a relative path at a specified speed, orienting the node to the path.

class func follow(CGPath, asOffset: Bool, orientToPath: Bool, duration: TimeInterval) -> SKAction

Creates an action that moves the node along a path.

class func follow(CGPath, asOffset: Bool, orientToPath: Bool, speed: CGFloat) -> SKAction

Creates an action that moves the node at a specified speed along a path.

### Animating the Rotation of a Node

Animate the z rotation of a node. If instead you wish to change the x or y rotation of a node, see SKTransformNode.

class func rotate(byAngle: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that rotates the node by a relative value.

class func rotate(toAngle: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that rotates the node counterclockwise to an absolute angle.

class func rotate(toAngle: CGFloat, duration: TimeInterval, shortestUnitArc: Bool) -> SKAction

Creates an action that rotates the node to an absolute value.

### Controlling the Action’s Speed

Control the speed of an animation.

class func speed(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes how fast the node executes actions by a relative value.

class func speed(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes how fast the node executes actions.

### Animating the Scaling of a Node

Animate the visual scaling of a node.

class func scale(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node by a relative value.

class func scale(to: CGSize, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node to achieve

class func scale(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node.

class func scaleX(by: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adds relative values to the x and y scale values of a node.

class func scaleX(to: CGFloat, y: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x and y scale values of a node.

class func scaleX(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the x scale value of a node to a new value.

class func scaleY(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the y scale value of a node to a new value.

### Animating the Transparency of a Node

Gradually change a node’s transparency.

class func fadeIn(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `1.0`.

class func fadeOut(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `0.0`.

class func fadeAlpha(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the alpha value of a node by a relative value.

class func fadeAlpha(to: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the alpha value of a node to a new value.

### Animating a Node’s Texture

Change a node’s texture or the texture’s properties.

class func resize(byWidth: CGFloat, height: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the size of a sprite.

class func resize(toHeight: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the height of a sprite to a new absolute value.

class func resize(toWidth: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the width of a sprite to a new absolute value.

class func resize(toWidth: CGFloat, height: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes the width and height of a sprite to a new absolute value.

class func setTexture(SKTexture) -> SKAction

Creates an action that changes a sprite’s texture.

class func setTexture(SKTexture, resize: Bool) -> SKAction

Creates an action that changes a sprite’s texture, possibly resizing the sprite.

class func animate(with: [SKTexture], timePerFrame: TimeInterval) -> SKAction

Creates an action that animates changes to a sprite’s texture.

class func animate(with: [SKTexture], timePerFrame: TimeInterval, resize: Bool, restore: Bool) -> SKAction

Creates an action that animates changes to a sprite’s texture, possibly resizing the sprite.

class func setNormalTexture(SKTexture) -> SKAction

Creates an action that changes a sprite’s normal texture.

class func setNormalTexture(SKTexture, resize: Bool) -> SKAction

Creates an action that changes a sprite’s normal texture, possibly resizing the sprite.

class func animate(withNormalTextures: [SKTexture], timePerFrame: TimeInterval) -> SKAction

Creates an action that animates changes to a sprite’s normal texture.

class func animate(withNormalTextures: [SKTexture], timePerFrame: TimeInterval, resize: Bool, restore: Bool) -> SKAction

Creates an action that animates changes to a sprite’s texture.

class func colorize(with: UIColor, colorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an animation that animates a sprite’s color and blend factor.

class func colorize(withColorBlendFactor: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that animates a sprite’s blend factor.

### Animating Properties of a Node’s Physics Body

Physics actions are instantaneous and therefore more useful when `Chaining Actions` or Reuse Actions.

class func applyForce(CGVector, duration: TimeInterval) -> SKAction

Creates an action that applies a force to the center of gravity of a node’s physics body.

class func applyTorque(CGFloat, duration: TimeInterval) -> SKAction

Creates an action that applies a torque to a node’s physics body.

class func applyForce(CGVector, at: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that applies a force to a specific point on a node’s physics body.

class func applyImpulse(CGVector, duration: TimeInterval) -> SKAction

Creates an action that applies an impulse to the center of gravity of a physics body.

class func applyAngularImpulse(CGFloat, duration: TimeInterval) -> SKAction

Creates an action that applies an angular impulse to a node’s physics body.

class func applyImpulse(CGVector, at: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that applies an impulse to a specific point of a node’s physics body.

class func applyImpulse(CGVector, duration: TimeInterval) -> SKAction

Creates an action that applies an impulse to the center of gravity of a physics body.

class func changeCharge(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the charge of a node’s physics body to a new value.

class func changeCharge(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the charge of a node’s physics body by a relative value.

class func changeMass(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the mass of a node’s physics body to a new value.

class func changeMass(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the mass of a node’s physics body by a relative value.

class func strength(to: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s strength.

class func strength(by: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s strength to a value relative to the existing value.

class func falloff(to: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s falloff.

class func falloff(by: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s falloff to a value relative to the existing value.

### Reversing an Animation

Create a new action that is the opposite of another action.

func reversed() -> SKAction

Creates an action that reverses the behavior of another action.

### Animate the Warping of a Node

Interpolate the warping of a node over time.

class func animate(withWarps: [SKWarpGeometry], times: [NSNumber]) -> SKAction?

Creates an action to distort a node through a sequence of SKWarpGeometry objects.

class func animate(withWarps: [SKWarpGeometry], times: [NSNumber], restore: Bool) -> SKAction?

Creates an action to distort a node through a sequence of SKWarpGeometry objects.

class func warp(to: SKWarpGeometry, duration: TimeInterval) -> SKAction?

Creates an action to distort a node based using an SKWarpGeometry object.

### Controlling the Audio of a Node

Audio actions are instantaneous and so, more useful when `Chaining Actions` or Reuse Actions.

class func playSoundFileNamed(String, waitForCompletion: Bool) -> SKAction

Creates an action that plays a sound.

class func play() -> SKAction

Creates an action that tells an audio node to start playback.

class func pause() -> SKAction

Creates an action that tells an audio node to pause playback.

class func stop() -> SKAction

Creates an action that tells an audio node to stop playback.

class func changePlaybackRate(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s playback rate to a new value.

class func changePlaybackRate(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s playback rate by a relative amount.

class func changeVolume(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s volume to a new value.

class func changeVolume(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s volume by a relative value.

class func changeObstruction(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s obstruction to a new value.

class func changeObstruction(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s obstruction by a relative value.

class func changeOcclusion(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s occlusion to a new value.

class func changeOcclusion(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s occlusion by a relative value.

class func changeReverb(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s reverb to a new value.

class func changeReverb(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s reverb by a relative value.

class func stereoPan(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s stereo panning to a new value.

class func stereoPan(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes an audio node’s stereo panning by a relative value.

### Removing a Node from the Scene

Instantaneous action that is useful when `Chaining Actions` or Reuse Actions.

class func removeFromParent() -> SKAction

Creates an action that removes the node from its parent.

### Running Actions on Children

Run an action on a child node by its name.

class func run(SKAction, onChildWithName: String) -> SKAction

Creates an action that runs an action on a named child object.

### Chaining Actions

Create an action that contains a series, or chain, of other actions.

class func group([SKAction]) -> SKAction

Creates an action that runs a collection of actions in parallel.

class func sequence([SKAction]) -> SKAction

Creates an action that runs a collection of actions sequentially.

class func `repeat`(SKAction, count: Int) -> SKAction

Creates an action that repeats another action a specified number of times.

class func repeatForever(SKAction) -> SKAction

Creates an action that repeats another action forever.

### Delaying Actions

Delay a subseqent action in a sequence of other actions.

class func wait(forDuration: TimeInterval) -> SKAction

Creates an action that idles for a specified period of time.

class func wait(forDuration: TimeInterval, withRange: TimeInterval) -> SKAction

Creates an action that idles for a randomized period of time.

### Performing Inverse Kinematics

Working with Inverse Kinematics

Gain fine-tuned control of objects that are connected by joints.

class func reach(to: CGPoint, rootNode: SKNode, duration: TimeInterval) -> SKAction

Creates an action that performs an inverse kinematic reach.

class func reach(to: CGPoint, rootNode: SKNode, velocity: CGFloat) -> SKAction

Creates an action that performs an inverse kinematic reach.

class func reach(to: SKNode, rootNode: SKNode, duration: TimeInterval) -> SKAction

Creates an action that performs an inverse kinematic reach.

class func reach(to: SKNode, rootNode: SKNode, velocity: CGFloat) -> SKAction

Creates an action that performs an inverse kinematic reach.

### Creating Custom Actions

Provide code that implements your own action.

init?(named: String)

Creates an action of the given name from an action file.

init?(named: String, duration: TimeInterval)

Creates an action of the given name from an action file with a new duration.

init?(named: String, fromURL: URL)

Creates an action of the given name from an action file.

init?(named: String, fromURL: URL, duration: TimeInterval)

Creates an action of the given name from an action file with a new duration.

class func customAction(withDuration: TimeInterval, actionBlock: (SKNode, CGFloat) -> Void) -> SKAction

Creates an action that executes a block over a duration.

class func perform(Selector, onTarget: Any) -> SKAction

Creates an action that calls a method on an object.

class func run(() -> Void) -> SKAction

Creates an action that executes a block.

class func run(() -> Void, queue: dispatch_queue_t) -> SKAction

Creates an action that executes a block on a specific dispatch queue.

### Controlling Node Visibility

Control a node’s visibility.

class func unhide() -> SKAction

Creates an action that makes a node visible.

class func hide() -> SKAction

Creates an action that hides a node.

## See Also

### First Steps

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

