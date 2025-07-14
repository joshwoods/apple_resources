

- Foundation
- XMLDocument
-  XMLDocument.ContentKind 

Enumeration

# XMLDocument.ContentKind

Type used to define the kind of document content.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum ContentKind
```

## Overview

For possible values, see doc:xmldocument/document_content_types.

## Topics

### Enumeration Cases

case html

Outputs empty tags in HTML without a close tag, such as ``.

case text

Outputs the string value of the document by extracting the string values from all text nodes.

case xhtml

The document output is XHTML.

case xml

The default type of document content type, which is XML.

case html

Outputs empty tags in HTML without a close tag, such as ``.

case text

Outputs the string value of the document by extracting the string values from all text nodes.

case xhtml

The document output is XHTML.

case xml

The default type of document content type, which is XML.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Input and Output Options

Input and output options specifically intended for `NSXMLDocument` objects.

Document Content Types

Define document types.

