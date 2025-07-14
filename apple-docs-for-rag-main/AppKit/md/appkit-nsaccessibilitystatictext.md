

- AppKit
-  NSAccessibilityStaticText 

Protocol

# NSAccessibilityStaticText

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as static text.

macOS

``` source
protocol NSAccessibilityStaticText : NSAccessibilityElementProtocol
```

## Overview

Use this protocol when you want to represent short pieces of text, such as headers or labels. For longer blocks of text, use the NSAccessibilityNavigableStaticText protocol.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityAttributedString(for: NSRange) -> NSAttributedString?

Returns the attributed substring for the specified range of characters.

func accessibilityValue() -> String?

Returns the text that the accessibility element displays.

**Required**

func accessibilityVisibleCharacterRange() -> NSRange

Returns the range of visible characters in the document.

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSObjectProtocol

### Inherited By

- NSAccessibilityNavigableStaticText

### Conforming Types

- NSComboBox
- NSSearchField
- NSSecureTextField
- NSTextField
- NSTextView
- NSTokenField

## See Also

### Text

protocol NSAccessibilityNavigableStaticText

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as navigable static text.

