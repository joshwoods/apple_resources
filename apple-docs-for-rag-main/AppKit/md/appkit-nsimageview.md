

- AppKit
-  NSImageView 

Class

# NSImageView

A display of image data in a frame.

macOS

``` source
@MainActor
class NSImageView
```

## Overview

Image views can be static or editable. A static image view only displays the image that you specify. An editable image view object lets the user change the displayed image. You can also configure an image view to allow copying, pasting, deleting, and dragging of the image.

Note

An image view calls its action method only when the user drags an image into the image view’s bounds, and the image view must be editable to receive dragged images. If you want to display an image and respond to clicks in the image, use an NSButton object instead.

## Topics

### Creating the view

convenience init(image: NSImage)

### Configuring the cell

class NSImageCell

An `NSImageCell` object displays a single image (encapsulated in an NSImage object) in a frame. This class provides methods for choosing the frame and for aligning and scaling the image to fit the frame.

### Specifying the image

var symbolConfiguration: NSImage.SymbolConfiguration?

var image: NSImage?

The image displayed by the image view.

### Specifying the visual characteristics

var imageFrameStyle: NSImageView.FrameStyle

The style of frame that appears around the image.

var imageAlignment: NSImageAlignment

The alignment of the cell’s image inside the image view.

var imageScaling: NSImageScaling

The scaling mode applied to make the cell’s image fit the frame of the image view.

var animates: Bool

A Boolean value indicating whether the image view automatically plays animated images.

var contentTintColor: NSColor?

### Specifying the dynamic range

var imageDynamicRange: NSImage.DynamicRange

The resolved dynamic range of the fully resolved image content.

var preferredImageDynamicRange: NSImage.DynamicRange

The preferred dynamic range when displaying an image in the receiving image view.

class var defaultPreferredImageDynamicRange: NSImage.DynamicRange

The default preferred image dynamic range.

### Responding to user events

var isEditable: Bool

A Boolean value indicating whether the user can drag a new image into the image view.

var allowsCutCopyPaste: Bool

A Boolean value indicating whether the image view lets the user cut, copy, and paste the image contents.

### Configuring symbol effects

func addSymbolEffect(some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds an indefinite symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete symbol effect to the image view with the specified options and animation.

func addSymbolEffect(some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Adds a discrete, indefinite symbol effect to the image view with the specified options and animation.

func setSymbolImage(NSImage, contentTransition: some ContentTransitionSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions)

Sets a symbol image using the specified content-transition effect and options.

func removeSymbolEffect(ofType: some IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; IndefiniteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete, indefinite effect type, using the specified options and animation setting.

func removeSymbolEffect(ofType: some DiscreteSymbolEffect &amp; SymbolEffect, options: SymbolEffectOptions, animated: Bool)

Removes the symbol effect that matches the specified discrete effect type, using the specified options and animation setting.

func removeAllSymbolEffects(options: SymbolEffectOptions, animated: Bool)

Removes all symbol effects from the image view, using the specified options and animation setting.

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
- NSAccessibilityImage
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSMenuItemValidation
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

