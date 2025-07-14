

- Foundation
- XMLElement
-  setChildren(\_:) 

Instance Method

# setChildren(\_:)

Sets all child nodes of the receiver at once, replacing any existing children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func setChildren(_ children: [XMLNode]?)
```

## Parameters 

`children`  

An array of `NSXMLElement` objects or XMLNode objects of kinds XMLNode.Kind.element, XMLNode.Kind.processingInstruction, XMLNode.Kind.text, or XMLNode.Kind.comment.

## Discussion

Send this message with `children` as `nil` to remove all child nodes.

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

func normalizeAdjacentTextNodesPreservingCDATA(Bool)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

