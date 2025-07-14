

- Foundation
- XMLNode
- XMLNode.Options
-  documentXInclude 

Type Property

# documentXInclude

Replaces all XInclude nodes in the document with the nodes referred to.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var documentXInclude: XMLNode.Options { get }
```

## Discussion

XInclude allows clients to include parts of another XML document within a document.

(Input)

## See Also

### Constants

static var documentTidyHTML: XMLNode.Options

Formats HTML into valid XHTML during processing of the document.

static var documentTidyXML: XMLNode.Options

Changes malformed XML into valid XML during processing of the document.

static var documentValidate: XMLNode.Options

Validates this document against its DTD (internal or external) or XML Schema.

static var documentIncludeContentTypeDeclaration: XMLNode.Options

Includes a content type declaration for HTML or XHTML in the output of the document.

