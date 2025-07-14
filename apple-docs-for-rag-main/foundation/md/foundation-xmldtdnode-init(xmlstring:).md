

- Foundation
- XMLDTDNode
-  init(xmlString:) 

Initializer

# init(xmlString:)

Returns an `NSXMLDTDNode` object initialized with the DTD declaration in a given string.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(xmlString string: String)
```

## Parameters 

`string`  

The DTD declaration.

## Return Value

An `NSXMLDTDNode` object initialized with the DTD declaration in `string`. Returns `nil` if initialization did not succeed, as might occur if the passed-in declaration is malformed.

## Discussion

The node kind (NSXMLNode) assigned to the returned object—element, attribute, entity, or notation declaration— is based on the full XML string that is parsed. To assign a subkind, set the dtdKind property.

You may also use the dtdNode(withXMLString:) or init(kind:) methods to create `NSXMLDTDNode` instances. However, you cannot use the latter method to create `NSXMLDTDNode` instances for attribute-list declarations.

## See Also

### Related Documentation

Tree-Based XML Programming Guide

