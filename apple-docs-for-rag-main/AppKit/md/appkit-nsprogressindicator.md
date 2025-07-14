

- AppKit
-  NSProgressIndicator 

Class

# NSProgressIndicator

An interface that provides visual feedback to the user about the status of an ongoing task.

macOS

``` source
@MainActor
class NSProgressIndicator
```

## Overview

Progress indicators can be determinate or indeterminate. A determinate indicator displays the completion percentage of a task. An indeterminate indicator shows that the app is busy without providing a visual indication of how long the task will take.

## Topics

### Animating the progress indicator

func startAnimation(Any?)

Starts the animation of an indeterminate progress indicator.

func stopAnimation(Any?)

Stops the animation of an indeterminate progress indicator.

var usesThreadedAnimation: Bool

A Boolean that indicates whether the progress indicator implements animation in a separate thread.

### Advancing the progress bar

func increment(by: Double)

Advances the progress bar of a determinate progress indicator by the specified amount.

var doubleValue: Double

The value that indicates the current extent of the progress indicator.

var minValue: Double

The minimum value for the progress indicator.

var maxValue: Double

The maximum value for the progress indicator.

### Observing the progress bar

var observedProgress: Progress?

The progress object to use for updating the progress view.

### Setting the appearance

var controlSize: NSControl.ControlSize

The size of the progress indicator.

var controlTint: NSControlTint

The progress indicator’s control tint.

Deprecated

var isBezeled: Bool

A Boolean that indicates whether the progress indicator’s frame has a three-dimensional bezel.

Deprecated

var isIndeterminate: Bool

A Boolean that indicates whether the progress indicator is indeterminate.

var style: NSProgressIndicator.Style

The style of the progress indicator (bar or spinning).

func sizeToFit()

This action method resizes the progress indicator to an appropriate size depending on the value of style.

var isDisplayedWhenStopped: Bool

A Boolean that indicates whether the progress indicator hides itself when it isn’t animating.

### Constants

enum Style

Constants that specify the progress indicator’s style.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityGroup
- NSAccessibilityProgressIndicator
- NSAccessibilityProtocol
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

class NSRuleEditor

An interface for configuring a rule-based list of options.

class NSPredicateEditor

A defined set of rules that allows the editing of predicate objects.

Search Field

Provide a text field that is optimized for text-based search interfaces.

class NSSegmentedControl

Display one or more buttons in a single horizontal group.

Slider

Display a range of values from which the user selects a single value.

