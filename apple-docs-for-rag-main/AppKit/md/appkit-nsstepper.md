

- AppKit
-  NSStepper 

Class

# NSStepper

An interface with up and down arrow buttons for incrementing or decrementing a value.

macOS

``` source
@MainActor
class NSStepper
```

## Overview

A stepper consists of two small arrows that can increment and decrement a value that appears beside it, such as a date or time. The illustration below shows a stepper to the right of a text field, which would show the stepper’s value.

The `NSStepper` class uses the NSStepperCell class to implement its user interface.

## Topics

### Configuring the Cell

class NSStepperCell

An `NSStepperCell` object controls the appearance and behavior of an NSStepper object.

### Specifying value range

var maxValue: Double

The stepper’s maximum value.

var minValue: Double

The stepper’s minimum value.

var increment: Double

The amount by which the receiver changes with each increment or decrement.

### Specifying how the stepper responds

var autorepeat: Bool

A Boolean value that indicates how the stepper responds to mouse events.

var valueWraps: Bool

A Boolean value that indicates whether the stepper wraps around the minimum and maximum values.

## Relationships

### Inherits From

- NSControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAccessibilityStepper
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

