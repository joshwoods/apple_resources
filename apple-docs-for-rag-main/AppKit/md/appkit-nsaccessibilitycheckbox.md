

- AppKit
-  NSAccessibilityCheckBox 

Protocol

# NSAccessibilityCheckBox

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a checkbox.

macOS

``` source
protocol NSAccessibilityCheckBox : NSAccessibilityButton
```

## Overview

Use this protocol when you want a user interface element to behave like a checkbox—a control that toggles between an on state, an off state, and an optional mixed state—in the accessibility hierarchy.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityValue() -> NSNumber?

Returns the checkbox’s value.

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

protocol NSAccessibilityRadioButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a radio button.

protocol NSAccessibilitySwitch

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a switch.

