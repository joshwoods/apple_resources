

- Foundation
- XMLElement
-  normalizeAdjacentTextNodesPreservingCDATA(\_:) 

Instance Method

# normalizeAdjacentTextNodesPreservingCDATA(\_:)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

Mac Catalyst 13.0+macOS 10.0+

``` source
func normalizeAdjacentTextNodesPreservingCDATA(_ preserve: Bool)
```

## Parameters 

`preserve`  

true if CDATA sections are left alone as text nodes, false otherwise.

## Discussion

A text node with a value of an empty string is removed. When you process an input source of XML, adjacent text nodes are automatically normalized. You should invoke this method (with `preserve` as false) before using the XMLNode methods objects(forXQuery:constants:) or nodes(forXPath:).

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

func replaceChild(at: Int, with: XMLNode)

Replaces a child node at a specified location with another child node.

func setChildren([XMLNode]?)

Sets all child nodes of the receiver at once, replacing any existing children.

