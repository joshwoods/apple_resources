

- Core Spotlight
- CSSearchableItemAttributeSet
-  identifier 

Instance Property

# identifier

A formal identifier that references the document the item represents.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var identifier: String? { get set }
```

## See Also

### Describing documents

var audiences: [String]?

A class of entity for which the item is intended or useful.

var contentDescription: String?

A description of the item’s content.

var creator: String?

The name of the app that created the content.

var encodingApplications: [String]?

The name of the apps that converted the original content into a PDF stream.

var fileSize: NSNumber?

The size of the document file.

var fontNames: [String]?

An array of font names the document uses.

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

