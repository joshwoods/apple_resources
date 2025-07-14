

- Foundation
- XMLDTD
-  insertChild(\_:at:) 

Instance Method

# insertChild(\_:at:)

Inserts a child node in the receiver’s list of children at a specific location in the list.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insertChild(
    _ child: XMLNode,
    at index: Int
)
```

## Parameters 

`child`  

An XML-node object that represents the child to insert.

`index`  

An integer identifying the location in the receiver’s list of children to insert `child`. The indices of subsequent children in the list are incremented by one.

## See Also

### Manipulating Child Nodes

func addChild(XMLNode)

Adds a child node to the end of the list of existing children.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node at a particular location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child at a particular index with another child.

func setChildren([XMLNode]?)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

