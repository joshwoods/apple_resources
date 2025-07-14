

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  inlinePresentationIntent 

Type Property

# inlinePresentationIntent

An attribute that provides details for an inline Markdown element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let inlinePresentationIntent: NSAttributedString.Key
```

## Discussion

The value of this key is an NSNumber that contains a value from the InlinePresentationIntent type. This value indicates the Markdown formatting to apply to the range of text.

The system provides default visual treatments for ranges of text with this attribute. To replace the default visual treatment, remove this attribute and replace it with the formatting options you want.

## See Also

### Getting Markdown attribute keys

static let presentationIntentAttributeName: NSAttributedString.Key

An attribute that provides details for a block-level Markdown element.

static let markdownSourcePosition: NSAttributedString.Key

The position in a Markdown source string corresponding to some attributed text.

static let alternateDescription: NSAttributedString.Key

An alternate description for a URL or image.

static let imageURL: NSAttributedString.Key

The URL for an image in Markdown text.

