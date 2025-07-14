

- Core Spotlight
- CSSearchableItemAttributeSet
-  contentDescription 

Instance Property

# contentDescription

A description of the item’s content.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var contentDescription: String? { get set }
```

## Discussion

A description may consist of an abstract, table of contents, reference to a graphical representation of content, a free-text account of the content, or other matter.

## See Also

### Describing documents

var audiences: [String]?

A class of entity for which the item is intended or useful.

var creator: String?

The name of the app that created the content.

var encodingApplications: [String]?

The name of the apps that converted the original content into a PDF stream.

var fileSize: NSNumber?

The size of the document file.

var fontNames: [String]?

An array of font names the document uses.

var identifier: String?

A formal identifier that references the document the item represents.

var kind: String?

A description of the kind of document the item represents.

var pageCount: NSNumber?

The number of pages in the document.

var pageHeight: NSNumber?

The height of the document page, in points (72 points per inch).

var pageWidth: NSNumber?

The width of the document page, in points (72 points per inch).

var securityMethod: String?

The security method (a type of encryption) that protects the document file.

var subject: String?

The subject of the document.

var theme: String?

The theme of the document.

