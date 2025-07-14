

- SpriteKit
- SKNode
-  enumerateChildNodes(withName:using:) 

Instance Method

# enumerateChildNodes(withName:using:)

Searches the children of the receiving node to perform processing for nodes that share a name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func enumerateChildNodes(
    withName name: String,
    using block: @escaping (SKNode, UnsafeMutablePointer) -> Void
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func enumerateChildNodes(
    withName name: String,
    using block: @escaping (SKNode, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`name`  

The name to search for. This may be either the literal name of the node or a customized search string. See `Searching the Node Tree`.

`block`  

A block to execute on nodes that match the `name` parameter. The block has the signature `(node:` SKNode `, stop:` UnsafeMutablePointer `ObjCBool `>)`.

## Mentioned in 

Searching the Node Tree

## Discussion

This method enumerates the child array in order, searching for nodes whose names match the search parameter. The block is called once for each node that matches the name parameter.

The following Swift code shows how you could enumerate through the child nodes of a scene with a name containing the string `yellow`. Each matching node is hidden until the enumeration finds a node that also contains the string `triangle`. When this node is reached, `stop` is set to true and the processing stops.

Listing 1. Enumerating child nodes

```
scene.enumerateChildNodes(withName: "*yellow*") {
    (node, stop) in

    node.run(SKAction.hide())

    if let name = node.name, name.contains("triangle") {
        stop.initialize(to: true)
    }
}
```

You can also search by class name using enumerateChildNodes(withName:using:). However, for custom classes, you need to specify the fully annotated class name (i.e. the project name followed by the class name). The following Swift code shows a custom class, `SpaceshipNode`, based on SKSpriteNode, and created in a project named `SpaceGame`. The first search fails to return an instance of `SpaceshipNode` added as a child of `parentNode`:

Listing 2. Enumerating child nodes

```
class SpaceshipNode: SKSpriteNode {
}

let parentNode = SKNode()
let childNode = SpaceshipNode()
parentNode.addChild(childNode)

parentNode.enumerateChildNodes(withName: "SpaceshipNode") {
    node, _ in
    // Unannotated name, returns no results 
}

parentNode.enumerateChildNodes(withName: "SpaceGame.SpaceshipNode") {
    node, _ in
    // Annotated name, successfully returns `childNode` 
}

parentNode.enumerateChildNodes(withName: "SKSpriteNode") {
    node, _ in
    // Superclass name, successfully returns `childNode` 
}
```

## See Also

### Accessing Nodes by Name

Searching the Node Tree

Access nodes by name to avoid needing an instance variable.

var name: String?

The node’s assignable name.

func childNode(withName: String) -> SKNode?

Searches the children of the receiving node for a node with a specific name.

subscript(String) -> [SKNode]

Returns an array of nodes that match the name parameter.

