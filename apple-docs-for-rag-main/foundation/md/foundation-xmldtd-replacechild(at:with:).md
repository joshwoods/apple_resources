

- Foundation
- XMLDTD
-  replaceChild(at:with:) 

Instance Method

# replaceChild(at:with:)

Replaces a child at a particular index with another child.

Mac Catalyst 13.0+macOS 10.0+

``` source
func replaceChild(
    at index: Int,
    with node: XMLNode
)
```

## Parameters 

`index`  

An integer identifying the position of a node in the receiver’s list of child nodes.

`node`  

An XMLNode object to replace the object at `index`.

## Discussion

The replaced child node is released.

## See Also

### Manipulating Child Nodes

func addChild(XMLNode)

Adds a child node to the end of the list of existing children.

func insertChild(XMLNode, at: Int)

Inserts a child node in the receiver’s list of children at a specific location in the list.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node at a particular location in the receiver’s list of children.

func setChildren([XMLNode]?)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

