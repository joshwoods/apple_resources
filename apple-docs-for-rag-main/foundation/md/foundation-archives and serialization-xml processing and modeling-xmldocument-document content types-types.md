

- Foundation
- Archives and Serialization
- XML Processing and Modeling
- XMLDocument
-  Document Content Types 

API Collection

# Document Content Types

Define document types.

## Overview

You specify one of the NSXMLDocumentContentKind constants in documentContentKind to indicate the kind of content required for document output.

## Topics

### Constants

case xml

The default type of document content type, which is XML.

case xhtml

The document output is XHTML.

case html

Outputs empty tags in HTML without a close tag, such as ``.

case text

Outputs the string value of the document by extracting the string values from all text nodes.

## See Also

### Constants

Input and Output Options

Input and output options specifically intended for `NSXMLDocument` objects.

enum ContentKind

Type used to define the kind of document content.

