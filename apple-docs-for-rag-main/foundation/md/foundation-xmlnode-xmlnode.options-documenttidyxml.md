

- Foundation
- XMLNode
- XMLNode.Options
-  documentTidyXML 

Type Property

# documentTidyXML

Changes malformed XML into valid XML during processing of the document.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var documentTidyXML: XMLNode.Options { get }
```

## Discussion

It also eliminates “pretty-printing” formatting, such as leading tab characters. It does respect the `xml:space="preserve"` attribute.

(Input)

## See Also

### Constants

static var documentTidyHTML: XMLNode.Options

Formats HTML into valid XHTML during processing of the document.

static var documentValidate: XMLNode.Options

Validates this document against its DTD (internal or external) or XML Schema.

static var documentXInclude: XMLNode.Options

Replaces all XInclude nodes in the document with the nodes referred to.

static var documentIncludeContentTypeDeclaration: XMLNode.Options

Includes a content type declaration for HTML or XHTML in the output of the document.

