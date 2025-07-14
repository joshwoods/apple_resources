

- Foundation
- XMLDocument
-  removeChild(at:) 

Instance Method

# removeChild(at:)

Removes the child node of the receiver located at a specified position in its array of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeChild(at index: Int)
```

## Parameters 

`index`  

An integer identifying the position of an child in the receiver’s array. If `index` is less than zero or greater than the number of children minus one, an out-of-bounds exception is raised.

## Discussion

Subsequent children have their indexes decreased by one. The removed XMLNode object is autoreleased.

## See Also

### Adding and Removing Child Nodes

func addChild(XMLNode)

Adds a child node after the last of the receiver’s existing children.

func insertChild(XMLNode, at: Int)

Inserts a node object at specified position in the receiver’s array of children.

func insertChildren([XMLNode], at: Int)

Inserts an array of children at a specified position in the receiver’s array of children.

func replaceChild(at: Int, with: XMLNode)

Replaces the child node of the receiver located at a specified position in its array of children with another node.

func setChildren([XMLNode]?)

Sets the child nodes of the receiver.

