

- AppKit
-  NSColorPanel 

Class

# NSColorPanel

A standard user interface for selecting color in an app.

macOS

``` source
@MainActor
class NSColorPanel
```

## Overview

NSColorPanel provides a number of standard color selection modes and, with the NSColorPickingDefault and NSColorPickingCustom protocols, allows an app to add its own color selection modes. It also allows the user to save swatches containing frequently used colors.

## Topics

### Obtaining the Shared Color-Panel Object

class var shared: NSColorPanel

Returns the shared `NSColorPanel` instance, creating it if necessary.

class var sharedColorPanelExists: Bool

Returns a Boolean value indicating whether the `NSColorPanel` has been created already.

### Setting Color Picker Modes

class func setPickerMode(NSColorPanel.Mode)

Specifies the color panel’s initial picker.

var mode: NSColorPanel.Mode

The mode of the receiver the mode is one of the modes allowed by the color mask.

enum Mode

A type defined for the `enum` constants specifying color panel modes.

class func setPickerMask(NSColorPanel.Options)

Determines which color selection modes are available in an application’s `NSColorPanel`.

struct Options

The color modes that are enabled for a color panel.

### Configuring the Color Panel

var accessoryView: NSView?

The accessory view.

var isContinuous: Bool

A Boolean value indicating whether the receiver continuously sends the action message to the target.

func setAction(Selector?)

Sets the color panel’s action message.

func setTarget(Any?)

Sets the target of the receiver.

var showsAlpha: Bool

A Boolean value that indicates whether the receiver shows alpha values and an opacity slider.

### Managing Color Lists

func attachColorList(NSColorList)

Adds the list of `NSColor` objects specified to all the color pickers in the receiver that display color lists by invoking attachColorList(_:) on all color pickers in the application.

func detachColorList(NSColorList)

Removes the list of colors from all the color pickers in the receiver that display color lists by invoking detachColorList(_:) on all color pickers in the application.

### Setting Color

class func dragColor(NSColor, with: NSEvent, from: NSView) -> Bool

Drags a color into a destination view from the specified source view.

var color: NSColor

The color of the receiver.

### Getting Transparency Information

var alpha: CGFloat

The receiver’s current alpha value based on its opacity slider.

### Responding to a Color Change

protocol NSColorChanging

class let colorDidChangeNotification: NSNotification.Name

Posted when the color of the `NSColorPanel` is set, as when NSColorPanel is invoked.

## Relationships

### Inherits From

- NSPanel

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
- NSMenuItemValidation
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable

## See Also

### Color Panels

protocol NSColorPickingCustom

A set of methods that provides a way to add color pickers—custom user interfaces for color selection—to an app’s color panel.

protocol NSColorPickingDefault

A set of methods that provides basic behavior for a color picker.

class NSColorPicker

An abstract superclass that implements the default color picking protocol.

