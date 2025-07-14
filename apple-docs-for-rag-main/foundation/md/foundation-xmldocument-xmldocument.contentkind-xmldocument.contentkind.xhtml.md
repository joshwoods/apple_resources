

- Foundation
- XMLDocument
- XMLDocument.ContentKind
-  XMLDocument.ContentKind.xhtml 

Case

# XMLDocument.ContentKind.xhtml

The document output is XHTML.

Mac Catalyst 13.0+macOS 10.0+

``` source
case xhtml
```

## Discussion

This is set automatically if the `NSXMLDocumentTidyHTML` option is set and NSXML detects HTML.

## See Also

### Enumeration Cases

case html

Outputs empty tags in HTML without a close tag, such as ``.

case text

Outputs the string value of the document by extracting the string values from all text nodes.

case xml

The default type of document content type, which is XML.

case html

Outputs empty tags in HTML without a close tag, such as ``.

case text

Outputs the string value of the document by extracting the string values from all text nodes.

case xml

The default type of document content type, which is XML.

