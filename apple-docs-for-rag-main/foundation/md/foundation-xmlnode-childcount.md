

- Foundation
- XMLNode
-  childCount 

Instance Property

# childCount

Returns the number of child nodes the receiver has.

Mac Catalyst 13.0+macOS 10.0+

``` source
var childCount: Int { get }
```

## Discussion

This receiver should be an `NSXMLNode` object representing a document, element, or document type declaration. For performance reasons, use this method instead of getting the count from the array returned by children (for example, `[[thisNode children] count`\]).

## See Also

### Navigating the Tree of Nodes

var rootDocument: XMLDocument?

Returns the XMLDocument object containing the root element and representing the XML document as a whole.

var parent: XMLNode?

Returns the parent node of the receiver.

func child(at: Int) -> XMLNode?

Returns the child node of the receiver at the specified location.

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

