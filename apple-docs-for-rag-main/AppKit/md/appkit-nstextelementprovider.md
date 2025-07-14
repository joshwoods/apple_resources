

- AppKit
-  NSTextElementProvider 

Protocol

# NSTextElementProvider

A protocol the text content manager and its concrete subclasses conform to, which defines the interface for interacting with custom content types of a text document.

macOS 12.0+

``` source
protocol NSTextElementProvider : NSObjectProtocol
```

## Topics

### Accessing the range of the text element

var documentRange: NSTextRange

Describes the starting and ending locations for the document.

**Required**

### Accessing and updating the text

func enumerateTextElements(from: (any NSTextLocation)?, options: NSTextContentManager.EnumerationOptions, using: (NSTextElement) -> Bool) -> (any NSTextLocation)?

Enumerates text elements starting at the text location you provide.

**Required**

struct EnumerationOptions

Values that describe options for enumerating text layout fragments.

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new location from location with offset you provide.

func replaceContents(in: NSTextRange, with: [NSTextElement]?)

Replaces the characters specified by range with the text elements you provide.

**Required**

### Adjusting the range of the text element

func adjustedRange(from: NSTextRange, forEditingTextSelection: Bool) -> NSTextRange?

A method you implement if the location backing store requires manual adjustment after editing.

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the offset between the two specified locations.

### Controlling synchronization with the backing store

func synchronizeToBackingStore((((any Error)?) -> Void)?)

Synchronizes changes to the backing store.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextContentManager
- NSTextContentStorage

## See Also

### Content elements

Enriching your text in text views

Add exclusion paths, text attachments, and text lists to your text, and render it with text views.

class NSTextParagraph

A class that represents a single paragraph backed by an attributed string as the contents.

class NSTextListElement

A class that represents a text list node.

class NSTextElement

An abstract base class that represents the smallest units of text layout such as paragraphs or attachments.

