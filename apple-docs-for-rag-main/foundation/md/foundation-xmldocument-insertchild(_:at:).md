

- Foundation
- XMLDocument
-  insertChild(\_:at:) 

Instance Method

# insertChild(\_:at:)

Inserts a node object at specified position in the receiver’s array of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insertChild(
    _ child: XMLNode,
    at index: Int
)
```

## Parameters 

`child`  

The XMLNode object to be inserted. The added node must be an `NSXMLNode` object representing a comment, processing instruction, or the root element.

`index`  

An integer specifying the index of the children array to insert `child`. The indexes of children after the new child are incremented. If `index` is less than zero or greater than the number of children, an out-of-bounds exception is raised.

## See Also

### Adding and Removing Child Nodes

func addChild(XMLNode)

Adds a child node after the last of the receiver’s existing children.

func insertChildren([XMLNode], at: Int)

Inserts an array of children at a specified position in the receiver’s array of children.

func removeChild(at: Int)

Removes the child node of the receiver located at a specified position in its array of children.

func replaceChild(at: Int, with: XMLNode)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

func setChildren([XMLNode]?)

Sets the child nodes of the receiver.

