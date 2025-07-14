

- Foundation
- XMLDocument
-  documentContentKind 

Instance Property

# documentContentKind

Sets the kind of output content for the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
var documentContentKind: XMLDocument.ContentKind { get set }
```

## Parameters 

`kind`  

An `enum` constant identifying a kind of document content. The valid NSXMLDocumentContentKind constants are `NSXMLDocumentXMLKind`, `NSXMLDocumentXHTMLKind`, `NSXMLDocumentHTMLKind`, and `NSXMLDocumentTextKind`.

## Discussion

Most of the differences among document-content kind have to do with the handling of content-less tags such as ``.

## See Also

### Managing Document Attributes

var characterEncoding: String?

Sets the character encoding of the receiver to `encoding`,

var dtd: XMLDTD?

Returns an XMLDTD object representing the internal DTD associated with the receiver.

var isStandalone: Bool

Sets a Boolean value that specifies whether the receiver represents a standalone XML document.

var mimeType: String?

Returns the MIME type for the receiver.

var version: String?

Sets the version of the receiver’s XML.

