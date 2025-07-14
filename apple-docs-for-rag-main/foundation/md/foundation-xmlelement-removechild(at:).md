

- Foundation
- XMLElement
-  removeChild(at:) 

Instance Method

# removeChild(at:)

Removes the child node of the receiver identified by a given index.

Mac Catalyst 13.0+macOS 10.0+

``` source
func removeChild(at index: Int)
```

## Parameters 

`index`  

An integer identifying the node in the receiver’s list of children to remove. An exception is raised if `index` is out of bounds.

## Discussion

The XML node object is released upon removal. The indices of subsequent children are decremented by one.

## See Also

### Manipulating Child Elements

func addChild(XMLNode)

Adds a child node at the end of the receiver’s current list of children.

func insertChild(XMLNode, at: Int)

Inserts a new child node at a specified location in the receiver’s list of child nodes.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func replaceChild(at: Int, with: XMLNode)

Replaces a child node at a specified location with another child node.

func setChildren([XMLNode]?)

Sets all child nodes of the receiver at once, replacing any existing children.

func normalizeAdjacentTextNodesPreservingCDATA(Bool)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

