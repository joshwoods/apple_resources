

- SpriteKit
- SKNode
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns an array of nodes that match the name parameter.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
subscript(name: String) -> [SKNode] { get }
```

**watchOS**

``` source
subscript(name: String) -> [SKNode] { get }
```

## Parameters 

`name`  

The name to search for. This may be either the literal name of the node or a customized search string. See `Searching the Node Tree`.

## Return Value

An array of `SKNode` objects that match the name. If no matching nodes are found, an empty array is returned.

## Mentioned in 

Searching the Node Tree

## See Also

### Accessing Nodes by Name

Searching the Node Tree

Access nodes by name to avoid needing an instance variable.

var name: String?

The node’s assignable name.

func childNode(withName: String) -> SKNode?

Searches the children of the receiving node for a node with a specific name.

func enumerateChildNodes(withName: String, using: (SKNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Searches the children of the receiving node to perform processing for nodes that share a name.

