

- Foundation
- XMLDocument
-  setChildren(\_:) 

Instance Method

# setChildren(\_:)

Sets the child nodes of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setChildren(_ children: [XMLNode]?)
```

## Parameters 

`children`  

An array of XMLNode objects. Each of these objects must represent comments, processing instructions, or the root element; otherwise, an exception is raised. Pass in `nil` to remove all children.

## See Also

### Adding and Removing Child Nodes

func addChild(XMLNode)

Adds a child node after the last of the receiver’s existing children.

func insertChild(XMLNode, at: Int)

Inserts a node object at specified position in the receiver’s array of children.

func insertChildren([XMLNode], at: Int)

Inserts an array of children at a specified position in the receiver’s array of children.

func removeChild(at: Int)

Removes the child node of the receiver located at a specified position in its array of children.

func replaceChild(at: Int, with: XMLNode)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

