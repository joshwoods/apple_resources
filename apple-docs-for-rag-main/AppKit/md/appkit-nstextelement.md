

- AppKit
-  NSTextElement 

Class

# NSTextElement

An abstract base class that represents the smallest units of text layout such as paragraphs or attachments.

macOS 12.0+

``` source
class NSTextElement
```

## Topics

### Creating a text element

init(textContentManager: NSTextContentManager?)

Creates a new text element with the content manager you provide.

### Accessing the content manager

var textContentManager: NSTextContentManager?

The value that represents the current content manager.

### Accessing the text element range

var elementRange: NSTextRange?

A range value that represents the range of the element inside the document.

### Accessing text elements

var isRepresentedElement: Bool

A Boolean value that indicates whether this element is in the text layout.

var parent: NSTextElement?

A value that represents the parent element if this text element is a child of an enclosing element.

var childElements: [NSTextElement]

An array of zero or more child text elements.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSTextParagraph

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

class NSTextParagraph

A class that represents a single paragraph backed by an attributed string as the contents.

class NSTextListElement

A class that represents a text list node.

protocol NSTextElementProvider

A protocol the text content manager and its concrete subclasses conform to, which defines the interface for interacting with custom content types of a text document.

