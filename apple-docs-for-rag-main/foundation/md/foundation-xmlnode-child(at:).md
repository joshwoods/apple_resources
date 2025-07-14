

- Foundation
- XMLNode
-  child(at:) 

Instance Method

# child(at:)

Returns the child node of the receiver at the specified location.

Mac Catalyst 13.0+macOS 10.0+

``` source
func child(at index: Int) -> XMLNode?
```

## Parameters 

`index`  

An integer specifying a node position in the receiver’s array of children. If `index` is out of bounds, an exception is raised.

## Return Value

An NSXMLNode object or `nil` f the receiver has no children.

## Discussion

The receiver should be an `NSXMLNode` object representing a document, element, or document type declaration. The returned node object can represent an element, comment, text, or processing instruction.

## See Also

### Navigating the Tree of Nodes

var rootDocument: XMLDocument?

Returns the XMLDocument object containing the root element and representing the XML document as a whole.

var parent: XMLNode?

Returns the parent node of the receiver.

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

