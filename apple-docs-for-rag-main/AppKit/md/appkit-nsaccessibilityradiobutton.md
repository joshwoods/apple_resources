

- AppKit
-  NSAccessibilityRadioButton 

Protocol

# NSAccessibilityRadioButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a radio button.

macOS

``` source
protocol NSAccessibilityRadioButton : NSAccessibilityButton
```

## Overview

Use this protocol when you want a user interface element to behave like a radio button—a control for constraining a selection to a single element from several elements—in the accessibility hierarchy.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityValue() -> NSNumber?

Returns the radio button’s value.

**Required**

## Relationships

### Inherits From

- NSAccessibilityButton
- NSAccessibilityElementProtocol
- NSObjectProtocol

## See Also

### Buttons

protocol NSAccessibilityButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a button.

protocol NSAccessibilitySwitch

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a switch.

protocol NSAccessibilityCheckBox

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a checkbox.

