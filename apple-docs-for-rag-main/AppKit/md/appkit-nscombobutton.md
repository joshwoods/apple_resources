

- AppKit
-  NSComboButton 

Class

# NSComboButton

A button with a pull-down menu and a default action.

macOS 13.0+

``` source
@MainActor
class NSComboButton
```

## Overview

An NSComboButton object is a button that displays a title string, image, and an optional control for displaying a menu. Use this control in places where you want to offer a button with a default action and one or more alternative actions. Clicking the title or image executes the default action you provide, and clicking the menu control displays a menu for selecting a different action. If you configure the button to hide the menu control, a long-press gesture displays the menu.

After you create a combo button programmatically or in Interface Builder, choose the button style you want and add a title or image for your content. A combo button has a default action, which you specify at creation time. You can also change that action later using the inherited target and action properties. To specify one or more alternative actions, configure a menu with those actions and assign it to the button’s menu property.

This control doesn’t use an NSCell object for its underlying implementation. It also doesn’t support the addition of a contextual menu.

## Topics

### Creating a Combo Button

convenience init(title: String, image: NSImage, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays both a title and image.

convenience init(title: String, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays a title.

convenience init(image: NSImage, menu: NSMenu?, target: Any?, action: Selector?)

Creates a combo button that displays an image.

### Configuring the Button Appearance

var style: NSComboButton.Style

The appearance setting that determines how the button presents its menu .

enum Style

Constants that indicate how a combo button presents its menu.

var title: String

The localized string that the button displays.

var image: NSImage?

The image that the button displays.

var imageScaling: NSImageScaling

The scaling behavior to apply to the button’s image.

### Specifying the Alternative Actions

var menu: NSMenu

The menu that contains the button’s alternate actions.

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

Slider

Display a range of values from which the user selects a single value.

