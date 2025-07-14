

- Foundation
- XMLNode
-  children 

Instance Property

# children

Returns an immutable array containing the child nodes of the receiver (as `NSXMLNode` objects).

Mac Catalyst 13.0+macOS 10.0+

``` source
var children: [XMLNode]? { get }
```

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

