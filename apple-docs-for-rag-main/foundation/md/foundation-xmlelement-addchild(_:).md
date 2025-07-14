

- Foundation
- XMLElement
-  addChild(\_:) 

Instance Method

# addChild(\_:)

Adds a child node at the end of the receiver’s current list of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func addChild(_ child: XMLNode)
```

## Parameters 

`child`  

An XML node object to add to the receiver’s children.

## Discussion

The new node has an index value that is one greater than the last of the current children.

## See Also

### Manipulating Child Elements

func insertChild(XMLNode, at: Int)

Inserts a new child node at a specified location in the receiver’s list of child nodes.

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

