

- SceneKit
-  SCNAction 

Class

# SCNAction

A simple, reusable animation that changes attributes of any node you attach it to.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNAction
```

## Overview

You use actions most often to change the structure and content of the SCNNode object to which they are attached, but you can also use actions to make other changes to the scene. In SceneKit, actions provide an easy way to implement animated behaviors that frequently change in response to user input.

### Working with Actions

To create an action, call the class method for the action you are interested in. Then, configure the action’s properties. Finally, to execute the action, call a node object’s run(_:) method (or a similar method from the SCNActionable protocol) and pass it the action object.

Most actions allow you to change a node’s properties, such as its position, rotation, or scale. Many of these actions are animated by SceneKit, meaning that they change the properties of the associated node over more than one frame of animation rendered by the scene. When an action is animated, the duration property states how long that action takes to complete in seconds and its timingMode property defines the rate at which the animation executes. The action’s speed property allows you to adjust the timing of the animation by increasing or decreasing its playback speed.

Many actions can be *reversed*, allowing you to create another action object that reverses the effect of that action. For example, if an action object moves a node `20` units in the positive X direction of its parent’s local coordinate space, the reversed action moves the node `20` units in the negative X direction. To create a reversed action object, call an action object’s reversed() method.

Some actions include other actions as children:

- A *sequence action* has multiple child actions. Each action in the sequence begins after the previous action ends.

- A *group action* has multiple child actions. All actions stored in the group begin executing at the same time.

- A *repeating action* stores a single child action. When the child action completes, it is restarted.

You can nest groups, sequences, and repeating actions. By combining actions together, you can add sophisticated behaviors to a node.

### Using Actions for Scene Animation

Actions are easily reused, can be added and removed while running, and directly affect presented nodes. For these reasons, actions work well when your scene changes frequently in response to user input—such as when building a game. Not all elements of a scene can be animated using actions. For other kinds of animation, use implicitly animated object properties (see the SCNTransaction class) or explicitly created Core Animation objects (see the SCNAnimatable protocol), or change the scene graph directly for each rendered frame (see the SCNSceneRendererDelegate protocol).

### Subclassing Notes

You never subclass SCNAction directly. Instead, create actions that call methods on arbitrary objects or execute blocks of code. See Creating Custom Actions.

## Topics

### Creating Actions That Move a Node

class func moveBy(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that moves a node relative to its current position.

class func move(by: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that moves a node relative to its current position.

class func move(to: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that moves a node to a new position.

### Creating Actions That Rotate a Node

class func rotateBy(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node in each of the three principal axes by angles relative to its current orientation.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotateTo(x: CGFloat, y: CGFloat, z: CGFloat, duration: TimeInterval, usesShortestUnitArc: Bool) -> SCNAction

Creates an action that rotates the node to absolute angles in each of the three principal axes.

class func rotate(by: CGFloat, around: SCNVector3, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node by an angle around a specified axis.

class func rotate(toAxisAngle: SCNVector4, duration: TimeInterval) -> SCNAction

Creates an action that rotates the node to an absolute angle around a specified axis.

### Creating Actions That Change a Node’s Scale

class func scale(by: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that uniformly changes the scale factor of a node by a relative value.

class func scale(to: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that uniformly changes the scale factor of a node to an absolute value.

### Creating Actions That Change a Node’s Opacity

class func fadeIn(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `1.0`.

class func fadeOut(duration: TimeInterval) -> SCNAction

Creates an action that changes the opacity of the node to `0.0`.

class func fadeOpacity(by: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that adjusts the opacity of a node by a relative value.

class func fadeOpacity(to: CGFloat, duration: TimeInterval) -> SCNAction

Creates an action that adjusts the opacity of a node to a new value.

### Creating Actions That Change a Node’s Visibility

class func hide() -> SCNAction

Creates an action that hides a node.

class func unhide() -> SCNAction

Creates an action that ensures a node is not hidden.

### Creating Actions That Remove Nodes from the Scene

class func removeFromParentNode() -> SCNAction

Creates an action that removes the node from its parent.

### Creating Actions That Play Audio

class func playAudio(SCNAudioSource, waitForCompletion: Bool) -> SCNAction

Creates an action that plays an audio source.

### Creating Actions That Combine or Repeat Other Actions

class func group([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions in parallel.

class func sequence([SCNAction]) -> SCNAction

Creates an action that runs a collection of actions sequentially.

class func `repeat`(SCNAction, count: Int) -> SCNAction

Creates an action that repeats another action a specified number of times.

class func repeatForever(SCNAction) -> SCNAction

Creates an action that repeats another action forever.

### Creating Actions That Add Delays to Action Sequences

class func wait(duration: TimeInterval) -> SCNAction

Creates an action that idles for a specified period of time.

class func wait(duration: TimeInterval, withRange: TimeInterval) -> SCNAction

Creates an action that idles for a randomized period of time.

### Creating Custom Actions

class func run((SCNNode) -> Void) -> SCNAction

Creates an action that executes a block.

class func run((SCNNode) -> Void, queue: dispatch_queue_t) -> SCNAction

Creates an action that executes a block on a specific dispatch queue.

class func customAction(duration: TimeInterval, action: (SCNNode, CGFloat) -> Void) -> SCNAction

Creates an action that executes a block periodically over a specified duration.

class func javaScriptAction(withScript: String, duration: TimeInterval) -> SCNAction

Creates an action that executes a JavaScript script periodically over a specified duration.

### Reversing an Action

func reversed() -> SCNAction

Creates an action that reverses the behavior of another action.

### Adjusting an Action’s Animation Properties

var duration: TimeInterval

The duration required to complete an action.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

var timingMode: SCNActionTimingMode

The timing mode used to execute an action.

var timingFunction: SCNActionTimingFunction?

A block SceneKit calls to determine the action’s animation timing.

### Constants

enum SCNActionTimingMode

Constants affecting the animation curve of an action, used by the timingMode property.

typealias SCNActionTimingFunction

The signature for a block that manages animation timing, used by the timingFunction property.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Actions

protocol SCNActionable

Methods for running actions on nodes.

