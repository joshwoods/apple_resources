

- SpriteKit
-  SKNode 

Class

# SKNode

The base class of all SpriteKit nodes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKNode
```

**watchOS**

``` source
class SKNode
```

## Mentioned in 

Customizing the Behavior of a Node

Controlling User Interaction on Nodes

Animate the Warping of a Sprite

Resizing a Sprite in Nine Parts

Searching the Node Tree

## Overview

`SKNode` provides base properties for its subclasses and it can be used as a container or layout tool for other nodes. For example, you might add a collection of nodes as children to an `SKNode` that all move together within the scene; because nodes inherit the properties of their parent, changing the parent node’s position propagates the change to its children as well.

`SKNode` does not draw any content itself. Its visual counterparts are listed in Nodes that Draw in Nodes for Scene Building.

## Topics

### First Steps

Getting Started with Nodes

Learn about the fundamental properties that provide a foundation for all other nodes.

init()

Initializes a blank node.

convenience init?(fileNamed: String)

Creates a new node by loading an archive file from the game’s main bundle.

init?(coder: NSCoder)

Called when a node is initialized from an .sks file.

convenience init(fileNamed: String, securelyWithClasses: Set&lt;AnyHashable>) throws

### Positioning Content in a Scene

Lay out content in a scene by positioning it within its parent’s coordinate system.

var position: CGPoint

The position of the node in its parent’s coordinate system.

### Querying the Content Size

Read the location and size of a node or its children in the parent’s coordinate space.

var frame: CGRect

A rectangle in the parent’s coordinate system that contains the node’s content, ignoring the node’s children.

func calculateAccumulatedFrame() -> CGRect

Returns a rectangle in the parent’s coordinate system that contains the position and size of itself and all child nodes.

### Configuring Draw Order

About Node Drawing Order

Understand how SpriteKit layers your scene’s nodes from top to bottom.

var zPosition: CGFloat

The height of the node relative to its parent.

### Scaling and Rotating

var zRotation: CGFloat

The Euler rotation about the z axis (in radians).

func setScale(CGFloat)

Sets the xScale and yScale properties of the node.

var xScale: CGFloat

A scaling factor that multiplies the width of a node and its children.

var yScale: CGFloat

A scaling factor that multiplies the height of a node and its children.

### Accessing Related Nodes

About SpriteKit Coordinate Systems

Learn how a node conforms to its coordinate systems.

var scene: SKScene?

The scene node that contains this node.

var parent: SKNode?

The node’s parent node.

var children: [SKNode]

The node’s children.

### Modifying the Node Tree

Accessing and Modifying the Node Tree

See the objects and functions you use to control the node tree’s composition.

func addChild(SKNode)

Adds a node to the end of the receiver’s list of child nodes.

func insertChild(SKNode, at: Int)

Inserts a node into a specific position in the receiver’s list of child nodes.

func isEqual(to: SKNode) -> Bool

Compares the parameter node to the receiving node.

func move(toParent: SKNode)

Moves the node to a new parent node in the scene.

func removeFromParent()

Removes the receiving node from its parent.

func removeAllChildren()

Removes all of the node’s children.

func removeChildren(in: [SKNode])

Removes a list of children from the receiving node.

func inParentHierarchy(SKNode) -> Bool

Returns a Boolean value that indicates whether the node is a descendant of the target node.

### Customizing Nodes

Customizing the Behavior of a Node

Organize your app’s logic and display code with nodes.

### Propagating Properties to Children

About Node Property Propagation

Learn which properties of a node affect its child nodes.

### Accessing Nodes by Name

Access nodes by name instead of instance properties.

Searching the Node Tree

Access nodes by name to avoid needing an instance variable.

var name: String?

The node’s assignable name.

func childNode(withName: String) -> SKNode?

Searches the children of the receiving node for a node with a specific name.

func enumerateChildNodes(withName: String, using: (SKNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Searches the children of the receiving node to perform processing for nodes that share a name.

subscript(String) -> [SKNode]

Returns an array of nodes that match the name parameter.

### Altering Node Visibility

Control whether a node is visible or semitransparent.

var alpha: CGFloat

The transparency value applied to the node’s contents.

var isHidden: Bool

A Boolean value that determines whether a node and its descendants are rendered.

### Running Actions

Run actions on a node and control their timing.

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

func run(SKAction)

Adds an action to the list of actions executed by the node.

func run(SKAction, completion: () -> Void)

Adds an action to the list of actions executed by the node and schedules the argument block to be run upon completion of the action.

func run(SKAction, withKey: String)

Adds an identifiable action to the list of actions executed by the node.

var speed: CGFloat

A speed modifier applied to all actions executed by a node and its descendants.

var isPaused: Bool

A Boolean value that determines whether actions on the node and its descendants are processed.

func action(forKey: String) -> SKAction?

Returns an action associated with a specific key.

func hasActions() -> Bool

Returns a Boolean value that indicates whether the node is executing actions.

func removeAllActions()

Ends and removes all actions from the node.

func removeAction(forKey: String)

Removes an action associated with a specific key.

### Adding Physics Behaviors

Enable physics behaviors by adding a body.

Getting Started with Physics Bodies

Create and assign a physics body to enable physics.

var physicsBody: SKPhysicsBody?

The physics body associated with the node.

### Constraining Node Position or Rotation

Define positional contraints relating to other nodes in the scene.

var constraints: [SKConstraint]?

A list of constraints to apply to the node.

var reachConstraints: SKReachConstraints?

The reach constraints to apply to the node when executing a reach action.

### Detecting Collisions Manually

As an alternative to SKPhysicsContactDelegate, manually check if two nodes overlap.

func intersects(SKNode) -> Bool

Returns a Boolean value that indicates whether this node intersects the specified node.

### Adding GameplayKit Behaviors

Enable GameplayKit behaviors by defining an entity and its obstacles in a scene.

var entity: GKEntity?

The GameplayKit entity this node represents.

class func obstacles(fromNodeBounds: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming its bounds into the scene’s coordinate system.

class func obstacles(fromNodePhysicsBodies: [SKNode]) -> [GKPolygonObstacle]

Converts each node into an obstacle by transforming the node’s physics body shape into the scene’s coordinate system.

class func obstacles(fromSpriteTextures: [SKNode], accuracy: Float) -> [GKPolygonObstacle]

Turns each node into an obstacle by changing the node’s texture into a physics shape and converting it into the scene’s coordinate system.

### Handling User Input

Enable user interaction to allow a node to respond to user input.

Controlling User Interaction on Nodes

Enable your node to respond to user input, like touches or mouse clicks.

var isUserInteractionEnabled: Bool

A Boolean value that indicates whether the node receives touch events.

var focusBehavior: SKNodeFocusBehavior

The focus behavior for a node.

### Hit Testing

Understanding Hit-Testing

Learn how find child nodes at a given point by using hit-testing.

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether a point lies inside the parent’s coordinate system.

func atPoint(CGPoint) -> SKNode

Returns the deepest visible descendant that intersects a point.

func nodes(at: CGPoint) -> [SKNode]

Returns an array of all visible descendants that intersect a point.

### Converting Between Coordinate Systems of Different Nodes

Converting Coordinate Spaces

Convert positions across the various coordinate spaces in a scene.

func convert(CGPoint, from: SKNode) -> CGPoint

Converts a point from the coordinate system of another node in the node tree to the coordinate system of this node.

func convert(CGPoint, to: SKNode) -> CGPoint

Converts a point in this node’s coordinate system to the coordinate system of another node in the node tree.

### Adding Custom Data Without Subclassing

Quickly add data to a node without having to subclass it.

var userData: NSMutableDictionary?

A dictionary containing arbitrary data.

### Providing Accessibility

Extend your app’s usability by exposing certain nodes in your scene as Accessibility user interface elements.

var accessibilityChildren: [Any]?

An array of user interface elements that represent children of this element.

var accessibilityFrame: CGRect

The size of this user interface element, in screen points.

var accessibilityHelp: String?

The help description of this user interface element; for example, the text shown in a tooltip.

var accessibilityLabel: String?

A short description of this user interface element.

var accessibilityParent: AnyObject?

The user interface element that contains this element.

var accessibilityRole: String?

A string value describing the user interface element type; for example, a button.

var accessibilityRoleDescription: String?

A string value describing the user interface element name and type; for example, the Buy button.

var accessibilitySubrole: String?

A string that defines this user interface element’s subrole; for example, a full-screen button.

var isAccessibilityElement: Bool

A toggle you implement to indicate to the system whether this user interface element should be exposed to the user.

var isAccessibilityEnabled: Bool

A toggle you implement to indicate to the system whether this user interface element should respond to user input.

func accessibilityHitTest(CGPoint) -> Any?

Returns the frontmost user interface element in the element hierarchy.

### Setting a Node’s Unique Attributes for a Shader

Set the values that make a node unique to a shader.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

Deprecated

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader

Deprecated

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

Deprecated

## Relationships

### Inherits From

- NSObject
- NSResponder
- UIResponder

### Inherited By

- SK3DNode
- SKAudioNode
- SKCameraNode
- SKCropNode
- SKEffectNode
- SKEmitterNode
- SKFieldNode
- SKLabelNode
- SKLightNode
- SKReferenceNode
- SKShapeNode
- SKSpriteNode
- SKTileMapNode
- SKTransformNode
- SKVideoNode

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
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Base Nodes

Using Base Nodes to Lay Out SpriteKit Content

Use nonvisual nodes to define the layout of a scene.

class SKCameraNode

A node that determines which parts of the scene are visible within a view.

class SKReferenceNode

A node that’s defined in an archived `.sks` file.

