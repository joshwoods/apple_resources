

- Foundation
- XMLDocument
-  version 

Instance Property

# version

Sets the version of the receiver’s XML.

Mac Catalyst 13.0+macOS 10.0+

``` source
var version: String? { get set }
```

## Parameters 

`version`  

A string object identifying the version of the XML.

## Discussion

Currently, the version should be either “1.0 “or “1.1”.

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

var mimeType: String?

Returns the MIME type for the receiver.

