

- Foundation
- XMLElement
-  insertChild(\_:at:) 

Instance Method

# insertChild(\_:at:)

Inserts a new child node at a specified location in the receiver’s list of child nodes.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insertChild(
    _ child: XMLNode,
    at index: Int
)
```

## Parameters 

`child`  

An XML node object to be inserted as a child of the receiver.

`index`  

An integer identifying a position in the receiver’s list of children. An exception is raised if `index` is out of bounds.

## Discussion

Insertion of the node increments the indexes of sibling nodes after it.

## See Also

### Manipulating Child Elements

func addChild(XMLNode)

Adds a child node at the end of the receiver’s current list of children.

func insertChildren([XMLNode], at: Int)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

func removeChild(at: Int)

Removes the child node of the receiver identified by a given index.

func replaceChild(at: Int, with: XMLNode)

Replaces a child node at a specified location with another child node.

func setChildren([XMLNode]?)

Sets all child nodes of the receiver at once, replacing any existing children.

func normalizeAdjacentTextNodesPreservingCDATA(Bool)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

