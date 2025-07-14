

- AppKit
-  NSLevelIndicator 

Class

# NSLevelIndicator

A visual representation of a level or quantity, using discrete values.

macOS

``` source
@MainActor
class NSLevelIndicator
```

## Overview

A level indicator is similar to an NSSlider object, but provides a more customized visual feedback to the user. Unlike sliders, level indicators do not have a “knob” indicating the current setting, and they do not allow the user to adjust the current setting. You set the value of the level indicator programmatically. The supported indicator styles include:

- A capacity style level indicator. The continuous mode for this style is often used to indicate conditions such as how much data is on hard disk. The discrete mode is similar to audio level indicators in audio playback applications. You can specify both a warning value and a critical value that provides additional visual feedback to the user.

- A ranking style level indicator. This is similar to the star ranking displays provided in iTunes and iPhoto. You can also specify your own ranking image.

- A relevancy style level indicator. This style is used to display the relevancy of a search result, for example in Mail.

`NSLevelIndicator` uses an NSLevelIndicatorCell to implement much of the control’s functionality. `NSLevelIndicator` provides cover methods for most of the NSLevelIndicatorCell methods, which call the corresponding cell method.

## Topics

### Configuring the Cell

class NSLevelIndicatorCell

`NSLevelIndicatorCell` is a subclass of NSActionCell that provides several level indicator display styles including: capacity, ranking and relevancy. The capacity style provides both continuous and discrete modes.

### Configuring the Range of Values

var minValue: Double

The receiver’s minimum value.

var maxValue: Double

The receiver’s maximum value.

var warningValue: Double

The receiver’s warning value.

var criticalValue: Double

The receiver’s critical value.

### Managing Tick Marks and Style

var tickMarkPosition: NSSlider.TickMarkPosition

Determines how the receiver’s tick marks are aligned with it.

var numberOfTickMarks: Int

The number of tick marks associated with the receiver.

var numberOfMajorTickMarks: Int

The number of major tick marks associated with the receiver.

func tickMarkValue(at: Int) -> Double

Returns the receiver’s value represented by the tick mark at the specified index (the minimum-value tick mark has an index of 0).

func rectOfTickMark(at: Int) -> NSRect

Returns the bounding rectangle of the tick mark identified by the specified index (the minimum-value tick mark is at index 0).

var levelIndicatorStyle: NSLevelIndicator.Style

The appearance of the indicator.

enum Style

Constants that specify a level indicator’s appearance.

### Configuring the Drawing Attributes

var ratingImage: NSImage?

var drawsTieredCapacityLevels: Bool

var fillColor: NSColor!

var warningFillColor: NSColor!

var criticalFillColor: NSColor!

### Managing Placeholder Information

var ratingPlaceholderImage: NSImage?

var placeholderVisibility: NSLevelIndicator.PlaceholderVisibility

enum PlaceholderVisibility

### Controlling the Edit Behavior

var isEditable: Bool

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

Slider

Display a range of values from which the user selects a single value.

