

- Foundation
- XMLNode
- XMLNode.Options
-  documentTidyHTML 

Type Property

# documentTidyHTML

Formats HTML into valid XHTML during processing of the document.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var documentTidyHTML: XMLNode.Options { get }
```

## Discussion

When tidying, `NSXMLDocument` adds a line break before the close tag of a block-level element (``, ``, ``, and so on); it also makes the string value of `` or `` a line break. These operations make the string value of the HTML `` more readable. After using this option, avoid outputting the document as anything other than the default kind, `NSXMLDocumentXHTMLKind`.

(Input)

## See Also

### Constants

static var documentTidyXML: XMLNode.Options

Changes malformed XML into valid XML during processing of the document.

static var documentValidate: XMLNode.Options

Validates this document against its DTD (internal or external) or XML Schema.

static var documentXInclude: XMLNode.Options

Replaces all XInclude nodes in the document with the nodes referred to.

static var documentIncludeContentTypeDeclaration: XMLNode.Options

Includes a content type declaration for HTML or XHTML in the output of the document.

