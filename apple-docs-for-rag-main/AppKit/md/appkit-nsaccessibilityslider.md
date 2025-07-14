

- AppKit
-  NSAccessibilitySlider 

Protocol

# NSAccessibilitySlider

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a slider.

macOS

``` source
protocol NSAccessibilitySlider : NSAccessibilityElementProtocol
```

## Overview

Use this protocol when you want a user interface element to behave like a slider—a control that represents a continuous range of numerical values with a knob that represents the currently selected value—in the accessibility hierarchy.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the slider.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the slider’s value.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the slider’s value.

**Required**

func accessibilityValue() -> Any?

Returns the slider’s value.

**Required**

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSObjectProtocol

### Conforming Types

- NSSlider

## See Also

### Value Controls

protocol NSAccessibilityStepper

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a stepper.

