

- AppKit
- Accessibility for AppKit
-  Custom Controls 

API Collection

# Custom Controls

Support accessibility for custom user interface elements by adopting a role-specific protocol and implementing its methods.

## Overview

Role-specific accessibility protocols represent the most common control types found in apps. Adopt a role-specific accessibility protocol if:

- You’re creating a custom control that’s a subclass of NSView, and you want to modify the control’s behavior beyond what AppKit provides by default.

- You’re working with a specialized control that doesn’t subclass NSView. See NSAccessibilityElement first.

First, identify the role-specific protocol that best matches your control’s intended behavior. For example, if your control is something that triggers actions when the user clicks it, adopt the NSAccessibilityButton protocol.

After you select an appropriate protocol, adopt that protocol. The compiler may ask you to reimplement some of the NSAccessibilityProtocol protocol’s accessor or action methods. Simply implement these methods, and your control is ready to use.

## Topics

### Buttons

protocol NSAccessibilityButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a button.

protocol NSAccessibilityRadioButton

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a radio button.

protocol NSAccessibilitySwitch

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a switch.

protocol NSAccessibilityCheckBox

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a checkbox.

### Value Controls

protocol NSAccessibilityStepper

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a stepper.

protocol NSAccessibilitySlider

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a slider.

### Groups

protocol NSAccessibilityGroup

A role-based protocol that declares the minimum interface necessary to act as a container for other user interface elements.

### Lists

protocol NSAccessibilityTable

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a table view.

protocol NSAccessibilityList

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a list view.

protocol NSAccessibilityOutline

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as an outline view.

protocol NSAccessibilityRow

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a row for a table, list, or outline view.

### Text

protocol NSAccessibilityStaticText

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as static text.

protocol NSAccessibilityNavigableStaticText

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as navigable static text.

### Images and Color

protocol NSAccessibilityImage

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as an image.

protocol NSAccessibilityColor

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a color.

### Loading

protocol NSAccessibilityProgressIndicator

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a progress indicator.

protocol NSAccessibilityElementLoading

A role-based protocol that declares the minimum interface necessary for an accessibility element to support loading.

### Dynamic Elements

protocol NSAccessibilityContainsTransientUI

A role-based protocol that declares the minimum interface necessary for an accessibility element to support dynamic UI changes.

### Layout Elements

protocol NSAccessibilityLayoutArea

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a layout area.

protocol NSAccessibilityLayoutItem

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a layout item.

### Supporting Types

protocol NSAccessibilityElementProtocol

A role-based protocol that declares the minimum interface necessary to interact with an assistive app.

## See Also

### Custom View Subclasses

Accessibility Functions

Global accessibility functions for custom views and controls.

