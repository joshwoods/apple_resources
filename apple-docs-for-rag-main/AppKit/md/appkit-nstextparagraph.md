

- AppKit
-  NSTextParagraph 

Class

# NSTextParagraph

A class that represents a single paragraph backed by an attributed string as the contents.

macOS 12.0+

``` source
class NSTextParagraph
```

## Topics

### Creating a paragraph

init(attributedString: NSAttributedString?)

Creates a new paragraph with the attributed string you provide.

### Getting paragraph characteristics

var attributedString: NSAttributedString

Returns the source attributed string.

var paragraphContentRange: NSTextRange?

Returns the range of the paragraph in the containing text’s attributed string.

var paragraphSeparatorRange: NSTextRange?

Returns the range of the paragraph separator in the containing text’s attributed string.

## Relationships

### Inherits From

- NSTextElement

### Inherited By

- NSTextListElement

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Content elements

Enriching your text in text views

Add exclusion paths, text attachments, and text lists to your text, and render it with text views.

class NSTextListElement

A class that represents a text list node.

class NSTextElement

An abstract base class that represents the smallest units of text layout such as paragraphs or attachments.

protocol NSTextElementProvider

A protocol the text content manager and its concrete subclasses conform to, which defines the interface for interacting with custom content types of a text document.

