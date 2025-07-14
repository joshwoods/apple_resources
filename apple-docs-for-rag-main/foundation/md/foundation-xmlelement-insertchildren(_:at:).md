

- Foundation
- XMLElement
-  insertChildren(\_:at:) 

Instance Method

# insertChildren(\_:at:)

Inserts an array of child nodes at a specified location in the receiver’s list of children.

Mac Catalyst 13.0+macOS 10.0+

``` source
func insertChildren(
    _ children: [XMLNode],
    at index: Int
)
```

## Parameters 

`children`  

An array of XML node objects to add as children of the receiver.

`index`  

An integer identifying a position in the receiver’s list of children. An exception is raised if `index` is out of bounds.

## Discussion

Insertion of the node increases the indexes of sibling nodes after it by the count of `children`.

## See Also

### Manipulating Child Elements

func addChild(XMLNode)

Adds a child node at the end of the receiver’s current list of children.

func insertChild(XMLNode, at: Int)

Inserts a new child node at a specified location in the receiver’s list of child nodes.

func removeChild(at: Int)

Removes the child node of the receiver identified by a given index.

func replaceChild(at: Int, with: XMLNode)

Replaces a child node at a specified location with another child node.

func setChildren([XMLNode]?)

Sets all child nodes of the receiver at once, replacing any existing children.

func normalizeAdjacentTextNodesPreservingCDATA(Bool)

Coalesces adjacent text nodes of the receiver that you have explicitly added, optionally including CDATA sections.

