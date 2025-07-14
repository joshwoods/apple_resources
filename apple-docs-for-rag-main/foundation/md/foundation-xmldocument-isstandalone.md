

- Foundation
- XMLDocument
-  isStandalone 

Instance Property

# isStandalone

Sets a Boolean value that specifies whether the receiver represents a standalone XML document.

Mac Catalyst 13.0+macOS 10.0+

``` source
var isStandalone: Bool { get set }
```

## Parameters 

`standalone`  

true if the receiver represents a standalone XML document, false otherwise.

## Discussion

A standalone document does not have an external DTD associated with it.

## See Also

### Managing Document Attributes

var characterEncoding: String?

Sets the character encoding of the receiver to `encoding`,

var documentContentKind: XMLDocument.ContentKind

Sets the kind of output content for the receiver.

var dtd: XMLDTD?

Returns an XMLDTD object representing the internal DTD associated with the receiver.

var mimeType: String?

Returns the MIME type for the receiver.

var version: String?

Sets the version of the receiver’s XML.

