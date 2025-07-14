

- Foundation
- XMLNode
-  xmlString(options:) 

Instance Method

# xmlString(options:)

Returns the string representation of the receiver as it would appear in an XML document, with one or more output options specified.

Mac Catalyst 13.0+macOS 10.0+

``` source
func xmlString(options: XMLNode.Options = []) -> String
```

## Parameters 

`options`  

One or more `enum` constants identifying an output option; bit-OR multiple constants together. See Constants for a list of valid constants for specifying output options.

## Discussion

The returned string includes the string representations of all children.

## See Also

### Emitting Node Content

var xmlString: String

Returns the string representation of the receiver as it would appear in an XML document.

func canonicalXMLStringPreservingComments(Bool) -> String

Returns a string object encapsulating the receiver’s XML in canonical form.

var description: String

