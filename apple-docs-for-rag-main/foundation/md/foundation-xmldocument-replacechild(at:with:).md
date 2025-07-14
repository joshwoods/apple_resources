

- Foundation
- XMLDocument
-  replaceChild(at:with:) 

Instance Method

# replaceChild(at:with:)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

Mac Catalyst 13.0+macOS 10.0+

``` source
func replaceChild(
    at index: Int,
    with node: XMLNode
)
```

## Parameters 

`index`  

An integer identifying a position in the receiver’s array of children. If `index` is less than zero or greater than the number of children minus one, an out-of-bounds exception is raised.

`node`  

An XMLNode object to replace the one at `index`; it must represent a comment, a processing instruction, or the root element.

## Discussion

The removed `NSXMLNode` object is autoreleased.

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

func setChildren([XMLNode]?)

Sets the child nodes of the receiver.

