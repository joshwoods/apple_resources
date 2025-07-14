

- AppKit
-  NSAccessibilityStepper 

Protocol

# NSAccessibilityStepper

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a stepper.

macOS

``` source
protocol NSAccessibilityStepper : NSAccessibilityElementProtocol
```

## Overview

Use this protocol when you want a user interface element to behave like a stepper—a control with up and down arrow buttons for incrementing or decrementing a value—in the accessibility hierarchy.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the stepper.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the stepper’s value.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the stepper’s value.

**Required**

func accessibilityValue() -> Any?

Returns the stepper’s value.

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSObjectProtocol

### Conforming Types

- NSStepper

## See Also

### Value Controls

protocol NSAccessibilitySlider

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a slider.

