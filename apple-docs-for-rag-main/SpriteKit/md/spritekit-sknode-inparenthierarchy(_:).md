

- SpriteKit
- SKNode
-  inParentHierarchy(\_:) 

Instance Method

# inParentHierarchy(\_:)

Returns a Boolean value that indicates whether the node is a descendant of the target node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func inParentHierarchy(_ parent: SKNode) -> Bool
```

**watchOS**

``` source
func inParentHierarchy(_ parent: SKNode) -> Bool
```

## Parameters 

`parent`  

An `SKNode` object to test against.

## Return Value

true if the node is a descendant of the `parent` node; otherwise false.

## See Also

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

