

- Foundation
- XMLNode
- XMLNode.Options
-  nodeCompactEmptyElement 

Type Property

# nodeCompactEmptyElement

Requests that an element should be contracted when empty; for example, ``.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var nodeCompactEmptyElement: XMLNode.Options { get }
```

## See Also

### Constants

static var documentIncludeContentTypeDeclaration: XMLNode.Options

Includes a content type declaration for HTML or XHTML in the output of the document.

static var documentTidyHTML: XMLNode.Options

Formats HTML into valid XHTML during processing of the document.

static var documentTidyXML: XMLNode.Options

Changes malformed XML into valid XML during processing of the document.

static var documentValidate: XMLNode.Options

Validates this document against its DTD (internal or external) or XML Schema.

static var documentXInclude: XMLNode.Options

Replaces all XInclude nodes in the document with the nodes referred to.

static var nodeExpandEmptyElement: XMLNode.Options

Requests that an element should be expanded when empty; for example, ``. This is the default.

static var nodeIsCDATA: XMLNode.Options

Specifies that a text node contains and is written out as a CDATA section.

static var nodeLoadExternalEntitiesAlways: XMLNode.Options

Requests that external entities are always loaded.

static var nodeLoadExternalEntitiesNever: XMLNode.Options

Requests that external entities are never loaded.

static var nodeLoadExternalEntitiesSameOriginOnly: XMLNode.Options

Requests that external entities are always loaded and only applies when a URL has been provided.

static var nodeNeverEscapeContents: XMLNode.Options

static var nodePreserveAll: XMLNode.Options

static var nodePreserveAttributeOrder: XMLNode.Options

Requests that NSXMLNode preserve the order of attributes as in the source XML.

static var nodePreserveCDATA: XMLNode.Options

Requests that NSXMLNode preserve CDATA blocks where defined in the input XML.

static var nodePreserveCharacterReferences: XMLNode.Options

Specifies that character references (`&#`*nnn*`;`) should not be resolved for XML output of this node.

