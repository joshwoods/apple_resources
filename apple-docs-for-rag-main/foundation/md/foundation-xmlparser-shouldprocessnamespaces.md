

- Foundation
- XMLParser
-  shouldProcessNamespaces 

Instance Property

# shouldProcessNamespaces

A Boolean value that determines whether the parser reports the namespaces and qualified names of elements.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var shouldProcessNamespaces: Bool { get set }
```

## Discussion

true if the parser reports namespace and qualified name, false otherwise.

The parser reports element names with the delegate methods parser(_:didStartElement:namespaceURI:qualifiedName:attributes:) and parser(_:didEndElement:namespaceURI:qualifiedName:).

## See Also

### Managing Parser Behavior

var shouldReportNamespacePrefixes: Bool

A Boolean value that determines whether the parser reports the prefixes indicating the scope of namespace declarations.

var shouldResolveExternalEntities: Bool

A Boolean value that determines whether the parser reports declarations of external entities.

