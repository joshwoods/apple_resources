

- Foundation
- XMLNode
-  detach() 

Instance Method

# detach()

Detaches the receiver from its parent node.

Mac Catalyst 13.0+macOS 10.0+

``` source
func detach()
```

## Discussion

This method is applicable to `NSXMLNode` objects representing elements, text, comments, processing instructions, attributes, and namespaces. Once the node object is detached, you can add it as a child node of another parent.

## See Also

### Navigating the Tree of Nodes

var rootDocument: XMLDocument?

Returns the XMLDocument object containing the root element and representing the XML document as a whole.

var parent: XMLNode?

Returns the parent node of the receiver.

func child(at: Int) -> XMLNode?

Returns the child node of the receiver at the specified location.

var childCount: Int

Returns the number of child nodes the receiver has.

var children: [XMLNode]?

Returns an immutable array containing the child nodes of the receiver (as `NSXMLNode` objects).

var next: XMLNode?

Returns the next `NSXMLNode` object in document order.

var nextSibling: XMLNode?

Returns the next `NSXMLNode` object that is a sibling node to the receiver.

var previous: XMLNode?

Returns the previous `NSXMLNode` object in document order.

var previousSibling: XMLNode?

Returns the previous `NSXMLNode` object that is a sibling node to the receiver.

