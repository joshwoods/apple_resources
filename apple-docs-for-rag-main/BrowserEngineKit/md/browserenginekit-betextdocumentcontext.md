

- BrowserEngineKit
-  BETextDocumentContext 

Class

# BETextDocumentContext

Information about the text surrounding a selection in a document.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
class BETextDocumentContext
```

## Mentioned in 

Integrating custom browser text views with UIKit

## Topics

### Creating a text document context

init(attributedSelectedText: NSAttributedString?, contextBefore: NSAttributedString?, contextAfter: NSAttributedString?, markedText: NSAttributedString?, selectedRangeInMarkedText: NSRange)

Initializes a new document context with attributed strings. The `selectedText`, `contextBefore`, and `contextAfter` represent the same ranges as they do in the `-initWithSelectedText:contextBefore:contextAfter:` initializer.

init(selectedText: String?, contextBefore: String?, contextAfter: String?, markedText: String?, selectedRangeInMarkedText: NSRange)

### Getting information about the selected range

var autocorrectedRanges: [NSValue]

Array of `NSRange` values, relative to the full context string made by combining the `contextBefore`, `markedText` (or `selectedText` if the marked text is empty), and the `contextAfter`.

### Adding text rectangles

func addTextRect(CGRect, forCharacterRange: NSRange)

Adds a text `rect` for the given character `range` The CGRects representing each character range are specified in -textInputView coordinates.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Replacements and AutoFill

class BEAutoFillTextSuggestion

class BETextAlternatives

class BETextDocumentRequest

struct Options

class BETextSuggestion

A text suggestion to insert into a document.

struct BETextReplacementOptions

