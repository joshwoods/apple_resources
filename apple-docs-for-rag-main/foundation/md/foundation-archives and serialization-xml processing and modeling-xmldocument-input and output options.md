

- Foundation
- Archives and Serialization
- XML Processing and Modeling
- XMLDocument
-  Input and Output Options 

API Collection

# Input and Output Options

Input and output options specifically intended for `NSXMLDocument` objects.

## Overview

Because `NSXMLDocument` is a subclass of XMLNode, you can also use the relevant input and output options described in Constants in the `NSXMLNode` class reference. You can specify input options in the `NSXMLDocument` methods init(contentsOf:options:), init(data:options:), init(xmlString:options:). The xmlData(options:) method takes output options.

## Topics

### Constants

static var documentTidyHTML: XMLNode.Options

Formats HTML into valid XHTML during processing of the document.

static var documentTidyXML: XMLNode.Options

Changes malformed XML into valid XML during processing of the document.

static var documentValidate: XMLNode.Options

Validates this document against its DTD (internal or external) or XML Schema.

static var documentXInclude: XMLNode.Options

Replaces all XInclude nodes in the document with the nodes referred to.

static var documentIncludeContentTypeDeclaration: XMLNode.Options

Includes a content type declaration for HTML or XHTML in the output of the document.

## See Also

### Constants

enum ContentKind

Type used to define the kind of document content.

Document Content Types

Define document types.

