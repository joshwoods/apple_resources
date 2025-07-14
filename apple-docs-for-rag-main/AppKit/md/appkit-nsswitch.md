

- AppKit
-  NSSwitch 

Class

# NSSwitch

A control that offers a binary choice.

macOS 10.15+

``` source
@MainActor
class NSSwitch
```

## Overview

The NSSwitch class provides a simple interface for displaying and toggling a Boolean state, such as on/off. A switch toggles its state and sends its action when clicked, activated through the keyboard, or tapped in the Touch Bar. NSSwitch also allows dragging between states, and if isContinuous is true, the switch sends its action for each change in position during the drag.

Use a switch to toggle significant preferences, or preferences that provide access to other controls. Avoid creating lists or tables of switches; instead, for general-purpose toggles, use an instance of NSButton to display a checkbox.

NSSwitch doesn’t use an instance of NSCell to provide its functionality. The cellClass class property and cell instance property both return Nil, and they ignore attempts to set a non-Nil value.

## Topics

### Managing Switch State

var state: NSControl.StateValue

The current position of the switch.

## Relationships

### Inherits From

- NSControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityButton
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAccessibilitySwitch
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Controls

Responding to control-based events using target-action

Handle user input by connecting buttons, sliders, and other controls to your app’s code using the target-action design pattern.

class NSButton

A control that defines an area on the screen that a user clicks to trigger an action.

class NSColorWell

A control that displays a color value and lets the user change that color value.

Combo Box

Display a list of values in a pop-up menu that lets the user select a value or type in a custom value.

class NSComboButton

A button with a pull-down menu and a default action.

Date Picker

Display a calendar date and provide controls for editing the date value.

class NSImageView

A display of image data in a frame.

class NSLevelIndicator

A visual representation of a level or quantity, using discrete values.

Path Control

A display of a file system path or virtual path information.

class NSPopUpButton

A control for selecting an item from a list.

class NSProgressIndicator

An interface that provides visual feedback to the user about the status of an ongoing task.

class NSRuleEditor

An interface for configuring a rule-based list of options.

class NSPredicateEditor

A defined set of rules that allows the editing of predicate objects.

Search Field

Provide a text field that is optimized for text-based search interfaces.

class NSSegmentedControl

Display one or more buttons in a single horizontal group.

