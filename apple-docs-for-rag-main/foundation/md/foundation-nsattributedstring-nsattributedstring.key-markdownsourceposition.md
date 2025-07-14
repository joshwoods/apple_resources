

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  markdownSourcePosition 

Type Property

# markdownSourcePosition

The position in a Markdown source string corresponding to some attributed text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let markdownSourcePosition: NSAttributedString.Key
```

## Discussion

This attribute indicates the position in the Markdown source where a run of attributed text begins and ends, omitting markup characters in the source. For example, after parsing the source string `“This is *emphasized*.”`, the text `emphasized` has a Markdown source position that starts at column `10`. This index is the `“e”` character, not the `“*”` formatting character.

An attributed string parsed from Markdown text includes this attribute only if the appliesSourcePositionAttributes value in the directory of NSAttributedString.DocumentReadingOptionKey options provided to the NSAttributedString initializer is `YES`.

## See Also

### Getting Markdown attribute keys

static let inlinePresentationIntent: NSAttributedString.Key

An attribute that provides details for an inline Markdown element.

static let presentationIntentAttributeName: NSAttributedString.Key

An attribute that provides details for a block-level Markdown element.

static let alternateDescription: NSAttributedString.Key

An alternate description for a URL or image.

static let imageURL: NSAttributedString.Key

The URL for an image in Markdown text.

