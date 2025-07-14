

- UIKit
-  NSTextListElement 

Class

# NSTextListElement

A class that represents a text list node.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
class NSTextListElement
```

## Topics

### Create a text list element

convenience init?(children: [NSTextListElement], textList: NSTextList, nestingLevel: Int)

Creates a text list element with the list elements and nesting level you provide.

convenience init(contents: NSAttributedString, markerAttributes: [NSAttributedString.Key : Any]?, textList: NSTextList, children: [NSTextListElement]?)

Creates a text list element with the list elements, nesting level, and marker attributes you provide.

init(parent: NSTextListElement?, textList: NSTextList, contents: NSAttributedString?, markerAttributes: [NSAttributedString.Key : Any]?, children: [NSTextListElement]?)

Creates a text list element with the parent, list elements, nesting level, and marker attributes you provide.

### Accessing the text elements

var textList: NSTextList

The value that represents the text list.

var parent: NSTextListElement?

A text list element that refers to the enclosing text list element.

var childElements: [NSTextListElement]

An array that contains child text elements.

### Accessing the text list’s attributes

var markerAttributes: [NSAttributedString.Key : Any]?

A dictionary of attributed string keys and IDs that represent the list’s marker attributes.

### Accessing the formatted string data

var attributedString: NSAttributedString

An attributed string that represents the string the framework displays for this element taking into account markers and the indentation level of the list element.

var contents: NSAttributedString?

The text list element contents without markers and formatting.

## Relationships

### Inherits From

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

class NSTextElement

An abstract base class that represents the smallest units of text layout such as paragraphs or attachments.

protocol NSTextElementProvider

A protocol the text content manager and its concrete subclasses conform to, which defines the interface for interacting with custom content types of a text document.

