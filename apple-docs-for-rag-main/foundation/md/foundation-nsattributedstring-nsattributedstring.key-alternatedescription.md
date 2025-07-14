

- Foundation
- NSAttributedString
- NSAttributedString.Key
-  alternateDescription 

Type Property

# alternateDescription

An alternate description for a URL or image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let alternateDescription: NSAttributedString.Key
```

## Discussion

The value of this key is an NSString with the alternate description of the URL or image.

When a Markdown link contains a title string, the system adds this key to the link text and sets the value to the title. For example, in the Markdown tect `[Visit the Apple Store](https://store.apple.com “The Apple Store website”)`, the system sets the value of this key to `The Apple Store website`.

## See Also

### Getting Markdown attribute keys

static let inlinePresentationIntent: NSAttributedString.Key

An attribute that provides details for an inline Markdown element.

static let presentationIntentAttributeName: NSAttributedString.Key

An attribute that provides details for a block-level Markdown element.

static let markdownSourcePosition: NSAttributedString.Key

The position in a Markdown source string corresponding to some attributed text.

static let imageURL: NSAttributedString.Key

The URL for an image in Markdown text.

