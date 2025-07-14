

- Foundation
- NSAttributedString
- NSAttributedString.DocumentAttributeKey
-  textLayoutSections 

Type Property

# textLayoutSections

The layout orientations for each section.

FoundationUIKitiOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let textLayoutSections: NSAttributedString.DocumentAttributeKey
```

## Discussion

An NSArray containing NSDictionary objects, each dictionary describing a layout orientation section. The dictionary can have two attributes: orientation and range. When there is a gap between sections, it’s assumed to have NSLayoutManager.TextLayoutOrientation.horizontal.

## See Also

### Getting document appearance keys

static let appearance: NSAttributedString.DocumentAttributeKey

The appearance of the document.

static let backgroundColor: NSAttributedString.DocumentAttributeKey

The background color of the document.

static let bottomMargin: NSAttributedString.DocumentAttributeKey

The bottom margin of the document.

static let defaultFontExcluded: NSAttributedString.DocumentAttributeKey

static let defaultTabInterval: NSAttributedString.DocumentAttributeKey

The default tab stop interval for the document.

static let excludedElements: NSAttributedString.DocumentAttributeKey

The HTML elements to exclude in generated HTML.

static let hyphenationFactor: NSAttributedString.DocumentAttributeKey

The hyphenation factor of the document.

static let leftMargin: NSAttributedString.DocumentAttributeKey

The left margin of the document.

static let paperMargin: NSAttributedString.DocumentAttributeKey

The paper margin of the document.

static let paperSize: NSAttributedString.DocumentAttributeKey

The paper size for the document.

static let prefixSpaces: NSAttributedString.DocumentAttributeKey

The number of spaces for indenting nested HTML elements.

static let rightMargin: NSAttributedString.DocumentAttributeKey

The right margin of the document.

static let topMargin: NSAttributedString.DocumentAttributeKey

The top margin of the document.

static let viewMode: NSAttributedString.DocumentAttributeKey

The view mode.

static let viewSize: NSAttributedString.DocumentAttributeKey

The view size.

