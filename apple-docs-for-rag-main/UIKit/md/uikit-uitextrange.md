

- UIKit
-  UITextRange 

Class

# UITextRange

A range of characters in a text container with a starting index and an ending index in string backing a text-entry object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITextRange
```

## Overview

Classes that adopt the UITextInput protocol must create custom UITextRange objects for representing ranges within the text managed by the class. The starting and ending indexes of the range are represented by UITextPosition objects. The text system uses both UITextRange and UITextPosition objects for communicating text-layout information. There are two reasons for using objects for text ranges rather than primitive types such as NSRange:

- Some documents contain nested elements (for example, HTML tags and embedded objects) and you need to track both absolute position and position in the visible text.

- The WebKit framework requires that text indexes and offsets be represented by objects.

If you adopt the UITextInput protocol, you must create a custom UITextRange subclass as well as a custom UITextPosition subclass.

## Topics

### Defining Ranges of Text

var start: UITextPosition

The start of a range of text.

var end: UITextPosition

The end of the range of text.

var isEmpty: Bool

A Boolean value that indicates whether the range of text represented by the receiver is zero-length.

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

class UITextSelectionRect

An encapsulation of information about a selected range of text in a document.

