

- Foundation
- XMLDTD
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds a child node to the end of the list of existing children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addChild(_ child: XMLNode)
```

## Parameters 

`child`  

The node object to add to the existing children.

## See Also

### Manipulating Child Nodes

func insertChild(XMLNode, at: Int)

Inserts a child node in the receiver’s list of children at a specific location in the list.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node at a particular location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child at a particular index with another child.

func setChildren([XMLNode]?)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

