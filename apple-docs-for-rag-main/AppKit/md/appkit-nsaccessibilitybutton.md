

- AppKit
-  NSAccessibilityButton 

Protocol

# NSAccessibilityButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a button.

macOS

``` source
protocol NSAccessibilityButton : NSAccessibilityElementProtocol
```

## Overview

Use this protocol when you want a user interface element to behave like a button—a control that triggers an action when the user clicks it—in the accessibility hierarchy.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the button.

**Required**

func accessibilityPerformPress() -> Bool

Simulates clicking the button.

**Required**

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSObjectProtocol

### Inherited By

- NSAccessibilityCheckBox
- NSAccessibilityRadioButton
- NSAccessibilitySwitch

### Conforming Types

- NSButton
- NSPopUpButton
- NSStatusBarButton
- NSSwitch

## See Also

### Buttons

protocol NSAccessibilityRadioButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a radio button.

protocol NSAccessibilitySwitch

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a switch.

protocol NSAccessibilityCheckBox

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a checkbox.

