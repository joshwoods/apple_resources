

- UIKit
-  UITextPosition 

Class

# UITextPosition

A position in a text container—that is, an index into the backing string in a text-display view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITextPosition
```

## Overview

Classes that adopt the UITextInput protocol must create custom UITextPosition objects for representing specific locations within the text managed by the class. The text input system uses both these objects and UITextRange objects for communicating text-layout information. There are two reasons for using objects for text positions rather than primitive types such as NSInteger:

- Some documents contain nested elements (for example, HTML tags and embedded objects) and you need to track both absolute position and position in the visible text.

- The WebKit framework requires that text indexes and offsets be represented by objects.

The simplest of UITextPosition objects—for example, one used in plain text—might have a single integer property that represents an offset into a string. If you adopt the UITextInput protocol, you must create a custom UITextRange subclass as well as a custom UITextPosition subclass.

This class declares no methods of its own.

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

class UITextRange

A range of characters in a text container with a starting index and an ending index in string backing a text-entry object.

class UITextSelectionRect

An encapsulation of information about a selected range of text in a document.

