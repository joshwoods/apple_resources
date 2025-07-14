

- Foundation
- XMLNode
-  parent 

Instance Property

# parent

Returns the parent node of the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
@NSCopying
var parent: XMLNode? { get }
```

## Discussion

Document nodes and standalone nodes (that is, the root of a detached branch of a tree) have no parent, and sending this message to them returns `nil`. A one-to-one relationship does not always exists between a parent and its children; although a namespace or attribute node cannot be a child, it still has a parent element.

## See Also

### Navigating the Tree of Nodes

var rootDocument: XMLDocument?

Returns the XMLDocument object containing the root element and representing the XML document as a whole.

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

func detach()

Detaches the receiver from its parent node.

