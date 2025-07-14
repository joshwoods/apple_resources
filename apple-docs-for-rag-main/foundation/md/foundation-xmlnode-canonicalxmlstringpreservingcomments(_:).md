

- Foundation
- XMLNode
-  canonicalXMLStringPreservingComments(\_:) 

Instance Method

# canonicalXMLStringPreservingComments(\_:)

Returns a string object encapsulating the receiver’s XML in canonical form.

Mac Catalyst 13.0+macOS 10.0+

``` source
func canonicalXMLStringPreservingComments(_ comments: Bool) -> String
```

## Parameters 

`comments`  

true to preserve comments, false otherwise.

## Discussion

Be sure to set the input option nodePreserveWhitespace for true canonical form. The canonical form of an XML document is defined by the World Wide Web Consortium at `http://www.w3.org/TR/xml-c14n`. Generally, if two documents with varying physical representations have the same canonical form, then they are considered logically equivalent within the given application context. The following list summarizes most key aspects of canonical form as defined by the W3C recommendation:

- Encodes the document in UTF-8.

- Normalizes line breaks to “#xA” on input before parsing.

- Normalizes attribute values in the manner of a validating processor.

- Replaces character and parsed entity references with their character content.

- Replaces CDATA sections with their character content.

- Removes the XML declaration and the document type declaration (DTD).

- Converts empty elements to start-end tag pairs.

- Normalizes whitespace outside of the document element and within start and end tags.

- Retains all whitespace characters in content (excluding characters removed during line-feed normalization).

- Sets attribute value delimiters to quotation marks (double quotes).

- Replaces special characters in attribute values and character content with character references.

- Removes superfluous namespace declarations from each element.

- Adds default attributes to each element.

- Imposes lexicographic order on the namespace declarations and attributes of each element.

## See Also

### Emitting Node Content

var xmlString: String

Returns the string representation of the receiver as it would appear in an XML document.

func xmlString(options: XMLNode.Options) -> String

Returns the string representation of the receiver as it would appear in an XML document, with one or more output options specified.

var description: String

