

- AppKit
-  NSAccessibilityNavigableStaticText 

Protocol

# NSAccessibilityNavigableStaticText

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as navigable static text.

macOS

``` source
protocol NSAccessibilityNavigableStaticText : NSAccessibilityStaticText
```

## Overview

Use this protocol when you want to represent larger blocks of text. The protocol allows users to navigate through the text a line at a time or a word at a time using an assistive app. For shorter pieces of text (for example, labels or headers), use the NSAccessibilityStaticText protocol instead.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityFrame(for: NSRange) -> NSRect

Returns the rectangle that encloses the specified range of characters.

**Required**

func accessibilityLine(for: Int) -> Int

Returns the line number for the line that contains the specified character index.

**Required**

func accessibilityRange(forLine: Int) -> NSRange

Returns the range of characters in the specified line.

**Required**

func accessibilityString(for: NSRange) -> String?

Returns the substring for the specified range.

**Required**

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSAccessibilityStaticText
- NSObjectProtocol

### Conforming Types

- NSComboBox
- NSSearchField
- NSSecureTextField
- NSTextField
- NSTextView
- NSTokenField

## See Also

### Text

protocol NSAccessibilityStaticText

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as static text.

