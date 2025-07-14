

- Foundation
- XMLDocument
-  mimeType 

Instance Property

# mimeType

Returns the MIME type for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var mimeType: String? { get set }
```

## Return Value

The MIME type for the receiver (for example, “text/xml”).

## Discussion

MIME types are assigned by IANA (see http://www.iana.org/assignments/media-types/index.html).

## See Also

### Managing Document Attributes

var characterEncoding: String?

Sets the character encoding of the receiver to `encoding`,

var documentContentKind: XMLDocument.ContentKind

Sets the kind of output content for the receiver.

var dtd: XMLDTD?

Returns an XMLDTD object representing the internal DTD associated with the receiver.

var isStandalone: Bool

Sets a Boolean value that specifies whether the receiver represents a standalone XML document.

var version: String?

Sets the version of the receiver’s XML.

