

- Foundation
- XMLDocument
-  dtd 

Instance Property

# dtd

Returns an XMLDTD object representing the internal DTD associated with the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
@NSCopying
var dtd: XMLDTD? { get set }
```

## Return Value

An XMLDTD object representing the internal DTD associated with the receiver or `nil` if no DTD has been associated.

## See Also

### Managing Document Attributes

var characterEncoding: String?

Sets the character encoding of the receiver to `encoding`,

var documentContentKind: XMLDocument.ContentKind

Sets the kind of output content for the receiver.

var isStandalone: Bool

Sets a Boolean value that specifies whether the receiver represents a standalone XML document.

var mimeType: String?

Returns the MIME type for the receiver.

var version: String?

Sets the version of the receiver’s XML.

