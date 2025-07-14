

- SpriteKit
- SKNode
-  childNode(withName:) 

Instance Method

# childNode(withName:)

Searches the children of the receiving node for a node with a specific name.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func childNode(withName name: String) -> SKNode?
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func childNode(withName name: String) -> SKNode?
```

## Parameters 

`name`  

The name to search for. This may be either the literal name of the node or a customized search string. See `Searching the Node Tree`.

## Return Value

If a node object with that name is found, the method returns the node object. Otherwise, it returns `nil`.

## Mentioned in 

Searching the Node Tree

## Discussion

If more than one child share the same name, the first node discovered is returned.

## See Also

### Accessing Nodes by Name

Searching the Node Tree

Access nodes by name to avoid needing an instance variable.

var name: String?

The node’s assignable name.

func enumerateChildNodes(withName: String, using: (SKNode, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Searches the children of the receiving node to perform processing for nodes that share a name.

subscript(String) -> [SKNode]

Returns an array of nodes that match the name parameter.

