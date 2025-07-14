

- Foundation
- XMLNode
-  description 

Instance Property

# description

Mac Catalyst 13.0+macOS 10.0+

``` source
var description: String { get }
```

## Discussion

```
@abstract Used for debugging. May give more information than XMLString.
```

## See Also

### Emitting Node Content

var xmlString: String

Returns the string representation of the receiver as it would appear in an XML document.

func xmlString(options: XMLNode.Options) -> String

Returns the string representation of the receiver as it would appear in an XML document, with one or more output options specified.

func canonicalXMLStringPreservingComments(Bool) -> String

Returns a string object encapsulating the receiver’s XML in canonical form.

