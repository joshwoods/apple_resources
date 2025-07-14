

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  presentationIntentAttributeName 

Type Property

# presentationIntentAttributeName

An attribute that provides details for a block-level Markdown element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let presentationIntentAttributeName: NSAttributedString.Key
```

## Discussion

The value of this key is an NSPresentationIntent object. Block-level elements include paragraphs, headers, lists, tables, and other structural elements of the Markdown content.

The system provides default visual treatments for ranges of text with this attribute. To replace the default visual treatment, remove this attribute and replace it with the formatting options you want.

## See Also

### Getting Markdown attribute keys

static let inlinePresentationIntent: NSAttributedString.Key

An attribute that provides details for an inline Markdown element.

static let markdownSourcePosition: NSAttributedString.Key

The position in a Markdown source string corresponding to some attributed text.

static let alternateDescription: NSAttributedString.Key

An alternate description for a URL or image.

static let imageURL: NSAttributedString.Key

The URL for an image in Markdown text.

