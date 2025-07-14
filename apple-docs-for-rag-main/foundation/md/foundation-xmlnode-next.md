

- Foundation
- XMLNode
-  next 

Instance Property

# next

Returns the next `NSXMLNode` object in document order.

Mac Catalyst 13.0+macOS 10.0+

``` source
@NSCopying
var next: XMLNode? { get }
```

## Discussion

You use this method to “walk” forward through the tree structure representing an XML document or document section. (Use previous to traverse the tree in the opposite direction.) Document order is the natural order that XML constructs appear in markup text. If you send this message to the last node in the tree, `nil` is returned. `NSXMLNode` bypasses namespace and attribute nodes when it traverses a tree in document order.

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

var nextSibling: XMLNode?

Returns the next `NSXMLNode` object that is a sibling node to the receiver.

var previous: XMLNode?

Returns the previous `NSXMLNode` object in document order.

var previousSibling: XMLNode?

Returns the previous `NSXMLNode` object that is a sibling node to the receiver.

func detach()

Detaches the receiver from its parent node.

