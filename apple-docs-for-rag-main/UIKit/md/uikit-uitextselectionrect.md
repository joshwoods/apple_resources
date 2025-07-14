

- UIKit
-  UITextSelectionRect 

Class

# UITextSelectionRect

An encapsulation of information about a selected range of text in a document.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITextSelectionRect
```

## Overview

This class is an abstract class and must be subclassed to be used. The system text input views provide their own concrete implementations of this class.

### Subclassing Notes

If you are implementing a custom text input view, you can subclass and use your custom class to return selection-related information. When subclassing, you should override and reimplement all properties. In your custom implementations, do not call `super`.

## Topics

### Accessing the Selection Rectangle

var rect: CGRect

The rectangle that encloses the text selection rectangle’s text range.

### Accessing Text-Related Attributes

var writingDirection: NSWritingDirection

The writing direction of text in the text selection rectangle’s text range.

var isVertical: Bool

A Boolean value that indicates whether the text is vertical.

### Determining the Selection Status

var containsStart: Bool

A Boolean value that indicates whether the rectangle contains the start of the selection.

var containsEnd: Bool

A Boolean value that indicates whether the rectangle contains the end of the selection.

### Instance Properties

var transform: CGAffineTransform

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
- Sendable

## See Also

### Metrics

class UITextPosition

A position in a text container—that is, an index into the backing string in a text-display view.

class UITextRange

A range of characters in a text container with a starting index and an ending index in string backing a text-entry object.

