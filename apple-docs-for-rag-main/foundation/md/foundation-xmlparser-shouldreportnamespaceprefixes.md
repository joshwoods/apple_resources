

- Foundation
- XMLParser
-  shouldReportNamespacePrefixes 

Instance Property

# shouldReportNamespacePrefixes

A Boolean value that determines whether the parser reports the prefixes indicating the scope of namespace declarations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var shouldReportNamespacePrefixes: Bool { get set }
```

## Discussion

true if the parser reports the scope of namespace declarations, false otherwise. The default value is false.

The parser reports prefixes with the delegate methods parser(_:didStartMappingPrefix:toURI:) and parser(_:didEndMappingPrefix:).

## See Also

### Managing Parser Behavior

var shouldProcessNamespaces: Bool

A Boolean value that determines whether the parser reports the namespaces and qualified names of elements.

var shouldResolveExternalEntities: Bool

A Boolean value that determines whether the parser reports declarations of external entities.

