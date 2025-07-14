

- Foundation
- XMLDTDNode
-  dtdKind 

Instance Property

# dtdKind

Returns the receiver’s DTD kind.

Mac Catalyst 13.0+macOS 10.0+

``` source
var dtdKind: XMLDTDNode.DTDKind { get set }
```

## Return Value

The receiver’s DTD kind. See Constants for a list of valid NSXMLDTDNodeKind constants.

## Discussion

The DTD kind is distinct from a `NSXMLDTDNode` object’s node kind (returned by the `NSXMLNode` kind method).

