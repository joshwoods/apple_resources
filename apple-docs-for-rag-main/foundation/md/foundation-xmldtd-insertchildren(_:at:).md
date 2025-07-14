

- Foundation
- XMLDTD
-  insertChildren(\_:at:) 

Instance Method

# insertChildren(\_:at:)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insertChildren(
    _ children: [XMLNode],
    at index: Int
)
```

## Parameters 

`children`  

An array of XMLNode objects to insert as children of the receiver.

`index`  

An integer identifying the location in the list of current children to make the insertion. The indices of subsequent children in the list are incremented by the number of inserted children.

## See Also

### Manipulating Child Nodes

func addChild(XMLNode)

Adds a child node to the end of the list of existing children.

func insertChild(XMLNode, at: Int)

Inserts a child node in the receiver’s list of children at a specific location in the list.

func removeChild(at: Int)

Removes the child node at a particular location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child at a particular index with another child.

func setChildren([XMLNode]?)

Removes all existing children of the receiver and replaces them with an array of new child nodes.

