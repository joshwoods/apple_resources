

- Foundation
- XMLNode
-  xmlString 

Instance Property

# xmlString

Returns the string representation of the receiver as it would appear in an XML document.

Mac Catalyst 13.0+macOS 10.0+

``` source
var xmlString: String { get }
```

## Discussion

The returned string includes the string representations of all children. This method invokes xmlString(options:) with an `options` argument of `NSXMLNodeOptionsNone`.

## See Also

### Emitting Node Content

func xmlString(options: XMLNode.Options) -> String

Returns the string representation of the receiver as it would appear in an XML document, with one or more output options specified.

func canonicalXMLStringPreservingComments(Bool) -> String

Returns a string object encapsulating the receiver’s XML in canonical form.

var description: String

