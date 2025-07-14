

- Foundation
- XMLElement
-  replaceChild(at:with:) 

Instance Method

# replaceChild(at:with:)

Replaces a child node at a specified location with another child node.

Mac Catalyst 13.0+macOS 10.0+

``` source
func replaceChild(
    at index: Int,
    with node: XMLNode
)
```

## Parameters 

`index`  

An integer identifying a position in the receiver’s list of children. An exception is raised if `index` is out of bounds.

`node`  

An XML node object that will replace the current child.

## Discussion

The replaced XML node object is released upon removal.

## See Also

### Manipulating Child Elements

func addChild(XMLNode)

Adds a child node at the end of the receiver’s current list of children.

func insertChild(XMLNode, at: Int)

Inserts a new child node at a specified location in the receiver’s list of child nodes.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node of the receiver identified by a given index.

func setChildren([XMLNode]?)

Sets all child nodes of the receiver at once, replacing any existing children.

func normalizeAdjacentTextNodesPreservingCDATA(Bool)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

