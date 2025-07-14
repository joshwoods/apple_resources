

- Foundation
- XMLDocument
-  characterEncoding 

Instance Property

# characterEncoding

Sets the character encoding of the receiver to `encoding`,

Mac Catalyst 13.0+macOS 10.0+

``` source
var characterEncoding: String? { get set }
```

## Parameters 

`encoding`  

A string that specifies an encoding; it must match the name of an IANA character set. See http://www.iana.org/assignments/character-sets for a list of valid encoding specifiers.

## Discussion

Typically the encoding is specified in the XML declaration of a document that is processed, but it can be set at any time. If the specified encoding does not match the actual encoding, parsing of the document might fail.

## See Also

### Managing Document Attributes

var documentContentKind: XMLDocument.ContentKind

Sets the kind of output content for the receiver.

var dtd: XMLDTD?

Returns an XMLDTD object representing the internal DTD associated with the receiver.

var isStandalone: Bool

Sets a Boolean value that specifies whether the receiver represents a standalone XML document.

var mimeType: String?

Returns the MIME type for the receiver.

var version: String?

Sets the version of the receiver’s XML.

