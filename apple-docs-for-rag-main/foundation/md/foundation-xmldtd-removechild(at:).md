

- Foundation
- XMLDTD
-  removeChild(at:) 

Instance Method

# removeChild(at:)

Removes the child node at a particular location in the receiver’s list of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeChild(at index: Int)
```

## Parameters 

`index`  

An integer identifying the child node to remove. The indices of subsequent children in the list are decremented by one.

## Discussion

The removed child node is released.

## See Also

### Manipulating Child Nodes

func addChild(XMLNode)

Adds a child node to the end of the list of existing children.

func insertChild(XMLNode, at: Int)

Inserts a child node in the receiver’s list of children at a specific location in the list.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child at a particular index with another child.

func setChildren([XMLNode]?)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

