

- AppKit
-  NSTextContentStorage 

Class

# NSTextContentStorage

A concrete object for managing your view’s text content and generating the text elements necessary for layout.

macOS 12.0+

``` source
class NSTextContentStorage
```

## Overview

An NSTextContentStorage object provides the backing store for a view that contains text. This object stores the text in an attributed string object, and defaults to using an NSTextStorage object. It also maps portions of the text to NSTextElement objects to organize the text into paragraphs, lists, and other common element types found in text content. During layout, TextKit uses these elements to lay out and render the text in your view.

The standard system views use an NSTextContentStorage object to manage their text content. When building a custom text view, use this type to store the text for your view. NSTextContentStorage works with an associated NSTextLayoutManager to lay out your view’s text. When someone inserts new text or edits the existing text, call the performEditingTransaction(_:) method and use a block to modify the contents of the attributedString property. Wrapping your edits in an edit transaction lets the rest of the text system respond to those changes.

TextKit uses the abstract NSTextLocation protocol to identify locations within text. NSTextContentStorage manager provides its own implementation of this protocol to represent locations within its storage object. To get the start and end locations, access the object’s documentRange property and use them to create new location objects. If you provide your own implementation of the NSTextLocation protocol to manage locations in your content, subclass NSTextContentManager and implement your own storage object to support those locations.

## Topics

### Managing the stored text

var attributedString: NSAttributedString?

An attributed string that contains the contents of the document.

### Accessing paragraphs

var delegate: (any NSTextContentStorageDelegate)?

The delegate for the content storage object.

protocol NSTextContentStorageDelegate

The optional methods that delegates of content storage objects implement to handle content processing.

### Finding ranges, locations, and offsets

func location(any NSTextLocation, offsetBy: Int) -> (any NSTextLocation)?

Returns a new text location object based on an existing location and offset you provide.

func offset(from: any NSTextLocation, to: any NSTextLocation) -> Int

Returns the number of characters between the specified locations.

func adjustedRange(from: NSTextRange, forEditingTextSelection: Bool) -> NSTextRange?

Returns the text range, if any, in the backing store that required manual adjustment after editing.

### Managing text elements

func textElement(for: NSAttributedString) -> NSTextElement?

Returns the text element corresponding to object’s attributed string.

func attributedString(for: NSTextElement) -> NSAttributedString?

Returns a new attributed string for the text element.

## Relationships

### Inherits From

- NSTextContentManager

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- NSTextElementProvider
- NSTextStorageObserving

## See Also

### Text management

class NSTextContentManager

An abstract class that defines the interface and a default implementation for managing the text document contents.

class NSAttributedString

A string of text that manages data, layout, and stylistic information for ranges of characters to support rendering.

class NSMutableAttributedString

A mutable string with associated attributes (such as visual style, hyperlinks, or accessibility data) for portions of its text.

