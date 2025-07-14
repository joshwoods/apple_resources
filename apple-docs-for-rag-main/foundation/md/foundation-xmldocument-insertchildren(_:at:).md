

- Foundation
- XMLDocument
-  insertChildren(\_:at:) 

Instance Method

# insertChildren(\_:at:)

Inserts an array of children at a specified position in the receiver’s array of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insertChildren(
    _ children: [XMLNode],
    at index: Int
)
```

## Parameters 

`children`  

An array of XMLNode objects representing comments, processing instructions, or the root element.

`index`  

An integer identifying the location in the receiver’s children array for insertion. The indexes of children after the new child are increased by `[children count`\]. If `index` is less than zero or greater than the number of children, an out-of-bounds exception is raised.

## See Also

### Adding and Removing Child Nodes

func addChild(XMLNode)

Adds a child node after the last of the receiver’s existing children.

func insertChild(XMLNode, at: Int)

Inserts a node object at specified position in the receiver’s array of children.

func removeChild(at: Int)

Removes the child node of the receiver located at a specified position in its array of children.

func replaceChild(at: Int, with: XMLNode)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

func setChildren([XMLNode]?)

Sets the child nodes of the receiver.

