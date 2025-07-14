

- AppKit
-  NSBox 

Class

# NSBox

A stylized rectangular box with an optional title.

macOS

``` source
@MainActor
class NSBox
```

## Overview

Use box objects to visually group the contents of your window. For example, you might use boxes to group related views. Use an NSBox object to configure the appearance of the box.

### Subclassing Notes

An `NSBox` object is a view that draws a line around its rectangular bounds and that displays a title on or near the line (or might display neither line nor title). You can adjust the style of the line (bezel, grooved, or plain) as well as the placement and font of the title. An `NSBox` also has a content view to which other views can be added; it thus offers a way for an application to group related views. You could create a custom subclass of `NSBox` that alters or augments its appearance or that modifies its grouping behavior. For example, you might add color to the lines or background, add a new line style, or have the views in the group automatically snap to an invisible grid when added.

#### Methods to Override

You must override the draw(_:) method (inherited from `NSView`) if you want to customize the appearance of your `NSBox` objects. Depending on the visual effect you’re trying to achieve, you may have to invoke `super`‘s implementation first. For example, if you are compositing a small image in a corner of the box, you would invoke the superclass implementation first. If you’re adding a new style of line, you would provide a way to store a request for this line type (such as a boolean instance variable and related accessor methods). Then, in draw(_:), if a request for this line type exists, you would draw the entire view yourself (that is, without calling `super`). Otherwise, you would invoke the superclass implementation.

If you wish to change grouping behavior or other behavioral characteristics of the `NSBox` class, consider overriding contentView, sizeToFit(), or addSubview(_:) (inherited from `NSView`).

#### Special Considerations

If you are drawing the custom `NSBox` entirely by yourself, and you want it to look exactly like the superclass object (except for your changes), it may take some effort and time to get the details right.

## Topics

### Configuring Boxes

var borderRect: NSRect

The rectangle in which the receiver’s border is drawn.

var boxType: NSBox.BoxType

The receiver’s box type.

var borderType: NSBorderType

The receiver’s border type.

Deprecated

var isTransparent: Bool

A Boolean value that indicates whether the receiver is transparent.

var title: String

The receiver’s title.

var titleFont: NSFont

The font object used to draw the receiver’s title.

var titlePosition: NSBox.TitlePosition

A constant representing the title position.

var titleCell: Any

The cell used to display the receiver’s title.

var titleRect: NSRect

The rectangle in which the receiver’s title is drawn.

### Customizing

var borderColor: NSColor

The color of the receiver’s border when the receiver is a custom box with a simple line border.

var borderWidth: CGFloat

The width of the receiver’s border when the receiver is a custom box with a simple line border.

var cornerRadius: CGFloat

The radius of the receiver’s corners when the receiver is a custom box with a simple line border.

var fillColor: NSColor

The color of the receiver’s background when the receiver is a custom box with a simple line border.

### Managing Content

var contentView: NSView?

The receiver’s content view.

var contentViewMargins: NSSize

The distances between the border and the content view.

### Sizing

func setFrameFromContentFrame(NSRect)

Places the receiver so its content view lies on the specified frame.

func sizeToFit()

Resizes and moves the receiver’s content view so it just encloses its subviews.

### Constants

enum TitlePosition

Specify the location of a box’s title with respect to its border.

enum BoxType

These constants and data type identifies box types, which, in conjunction with a box’s border type, define the appearance of the box.

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

### Visual Adornments

class NSVisualEffectView

A view that adds translucency and vibrancy effects to the views in your interface.

