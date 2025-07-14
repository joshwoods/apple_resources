

- AppKit
-  NSButtonCell 

Class

# NSButtonCell

An object that defines the user interface of a button or other clickable region of a view.

macOS

``` source
@MainActor
class NSButtonCell
```

## Overview

Setting the integer, float, double, or object value of an `NSButtonCell` object results in a call to state with the value converted to integer. In the case of objectValue, `nil` is equivalent to `0`, and a non-`nil` object that doesn’t respond to intValue sets the state to `1`. Otherwise, the state is set to the object’s intValue. Similarly, for most button types, querying the integer, float, double, or object value of an `NSButtonCell` returns the current state in the requested representation. In the case of objectValue, this is an `NSNumber` containing true for on, false for off, and integer value `-1` for the mixed state. For accelerator buttons (type NSAcceleratorButton or NSMultiLevelAcceleratorButton) on systems that support pressure sensitivity, querying doubleValue returns the amount of pressure applied while pressing the button.

The configuration of an NSButtonCell object controls how the button object appears and behaves, but it’s NSButton that sends a message when the control is clicked. For more information on the behavior of NSButtonCell, see the NSButton and NSMatrix class specifications, and Button Programming Topics.

### Exceptions

In its implementation of the compare(_:) method (declared in `NSCell`), `NSButtonCell` raises an `NSBadComparisonException` if the `otherCell` argument is not of the `NSButtonCell` class.

### Fonts

Setting the font property does nothing if the button has no title or alternate title. If the button cell has a key equivalent, its font is not changed, but the key equivalent’s font size is changed to match the new title font.

## Topics

### Creating the Cell

init(coder: NSCoder)

init(imageCell: NSImage?)

init(textCell: String)

### Setting Titles

var alternateTitle: String

The string displayed by the button when it’s in its alternate state.

var attributedAlternateTitle: NSAttributedString

The title displayed by the button when it’s in its alternate state, as an attributed string.

var attributedTitle: NSAttributedString

The title displayed by the button when it’s in its normal state as an attributed string.

var title: String!

The title displayed on the button when it’s in its normal state.

### Managing Images

var alternateImage: NSImage?

The image the button displays in its alternate state.

var imagePosition: NSControl.ImagePosition

The position of the button’s image relative to its title.

var imageScaling: NSImageScaling

The scale factor for the button’s image.

### Managing the Repeat Interval

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns by reference the delay and interval periods for a continuous button.

func setPeriodicDelay(Float, interval: Float)

Sets the message delay and interval for the button.

### Managing the Key Equivalent

var keyEquivalent: String

The button’s key-equivalent character.

var keyEquivalentFont: NSFont?

The font used to draw the button’s key equivalent.

Deprecated

var keyEquivalentModifierMask: NSEvent.ModifierFlags

The mask that identifies the modifier keys for the button’s key equivalent.

func setKeyEquivalentFont(String, size: CGFloat)

Sets by name and size of the font used to draw the key equivalent.

Deprecated

### Managing Graphics Attributes

var backgroundColor: NSColor?

The background color of the button.

var bezelStyle: NSButton.BezelStyle

The appearance of the button’s border, if it has one.

var gradientType: NSButton.GradientType

The gradient of the button’s border.

Deprecated

var imageDimsWhenDisabled: Bool

A Boolean value that indicates if the button’s image and text appear “dim” when the button is disabled.

var isOpaque: Bool

A Boolean value that indicates if the button is opaque.

var isTransparent: Bool

A Boolean value that indicates if the button is transparent.

var showsBorderOnlyWhileMouseInside: Bool

A Boolean value that indicates if the button displays its border only when the pointer is over it.

### Displaying the Cell

var highlightsBy: NSCell.StyleMask

A set of flags that indicate how the button highlights when it receives a mouse-down event (that is, when the button is pressed).

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

var showsStateBy: NSCell.StyleMask

The flags that indicate how the button cell shows its alternate state.

### Managing the Sound

var sound: NSSound?

The sound that’s played when the user presses the button (that is during a mouse-down event).

### Handling Events and Action Messages

func mouseEntered(with: NSEvent)

Draws the button’s border.

func mouseExited(with: NSEvent)

Erases the button’s border.

func performClick(Any?)

Simulates the user clicking the button with the pointer.

### Drawing the Button Content

func drawBezel(withFrame: NSRect, in: NSView)

Draws the border of the button using the current bezel style.

func drawImage(NSImage, withFrame: NSRect, in: NSView)

Draws the image associated with the button’s current state.

func drawTitle(NSAttributedString, withFrame: NSRect, in: NSView) -> NSRect

Draws the button’s title centered vertically in a specified rectangle.

### Constants

enum BezelStyle

The set of bezel styles to style buttons in your app.

enum ButtonType

Button types that you can specify using setButtonType(_:).

enum GradientType

Specify the gradients used by the gradientType property.

Deprecated

## Relationships

### Inherits From

- NSActionCell

### Inherited By

- NSMenuItemCell

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- Sendable

