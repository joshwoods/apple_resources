

- Foundation
- XMLDocument
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds a child node after the last of the receiver’s existing children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addChild(_ child: XMLNode)
```

## Parameters 

`child`  

The XMLNode object to be added.

## See Also

### Adding and Removing Child Nodes

func insertChild(XMLNode, at: Int)

Inserts a node object at specified position in the receiver’s array of children.

func insertChildren([XMLNode], at: Int)

Inserts an array of children at a specified position in the receiver’s array of children.

func removeChild(at: Int)

Removes the child node of the receiver located at a specified position in its array of children.

func replaceChild(at: Int, with: XMLNode)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

func setChildren([XMLNode]?)

Sets the child nodes of the receiver.

