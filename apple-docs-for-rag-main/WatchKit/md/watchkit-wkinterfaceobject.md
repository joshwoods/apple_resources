

- WatchKit
-  WKInterfaceObject 

Class

# WKInterfaceObject

An object that provides information that is common to all interface objects in your watchOS app.

watchOS 2.0+

``` source
class WKInterfaceObject
```

## Mentioned in 

Connecting Your User Interface to Your Code

## Overview

Your WatchKit extension uses interface objects to manipulate the visual elements displayed on Apple Watch. Specifically, you use the methods of this class to change the size, alignment, and visibility of those elements. You can also configure the accessibility information displayed through assistive technologies like VoiceOver.

Do not subclass or create instances of this class, or any of its subclasses, yourself. Instead, define outlets in your interface controller class and connect them to the corresponding objects in your storyboard file. For example, to refer to a button in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var button: WKInterfaceButton!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceButton* myButton;
```

At runtime, WatchKit creates the appropriate interface objects and assigns them to the outlets in your interface controller.

WatchKit provides one-way communication between the interface objects in your extension and the corresponding interface elements in your watchOS app. You can set the values of an interface object, but you cannot get the current values. If you want to know the current value of an attribute, you must save the value yourself.

### Interface Builder Configuration Options

Xcode lets you configure information about your group interface object in your storyboard file. The following table lists the attributes you can configure in your storyboard and their meaning.

| Attribute | Description |
|----|----|
| Alpha | The opacity of the object. A value of `1.0` represents fully opaque and a value of `0.0` represents fully transparent. |
| Hidden | A checkbox indicating whether the item is hidden initially. You can change the visibility of the item programmatically by calling the setHidden(_:) method. |
| Installed | A checkbox indicating whether the item is installed for the current device. |
| Horizontal | The horizontal alignment of the item. Use this attribute to configure the horizontal position of the item relative to its immediate parent. |
| Vertical | The vertical alignment of the item. Use this attribute to configure the vertical position of the item relative to its immediate parent. |
| Width | The width of the object. Specify a fixed width or set the value of the object to be a percentage of its container’s width. |
| Height | The height of the object. Specify a fixed height or set the value of the object to be a percentage of its container’s height. |

## Topics

### Hiding and Showing an Object

func setHidden(Bool)

Hides or shows the interface object in your user interface.

func setAlpha(CGFloat)

Sets the opacity of the interface object.

### Getting the Property Name

var interfaceProperty: String

The name of the outlet in your interface controller to which the object is bound.

### Changing an Object’s Size

func setWidth(CGFloat)

Sets the absolute width (in points) of the object.

func setHeight(CGFloat)

Sets the absolute height (in points) of the object.

func setRelativeWidth(CGFloat, withAdjustment: CGFloat)

Sets the width of the object relative to its container.

func setRelativeHeight(CGFloat, withAdjustment: CGFloat)

Sets the height of the object relative to its container.

func sizeToFitWidth()

Sets the width of the object to fit its current content.

func sizeToFitHeight()

Sets the height of the object so that it fills the available vertical space.

### Setting an Object’s Alignment

func setHorizontalAlignment(WKInterfaceObjectHorizontalAlignment)

Sets the horizontal alignment of an object relative to its container’s bounds.

func setVerticalAlignment(WKInterfaceObjectVerticalAlignment)

Sets the vertical alignment of an object relative to its container’s bounds.

### Configuring the Accessibility Attributes

func setAccessibilityIdentifier(String?)

Sets the unique identifier string for the interface object.

func setAccessibilityLabel(String?)

Sets a succinct label on the object that identifies the accessibility element.

func setAccessibilityHint(String?)

Sets the description of what happens when performing an action on the accessibility element.

func setAccessibilityValue(String?)

Sets the value of the accessibility element.

func setIsAccessibilityElement(Bool)

Sets whether the object is an accessibility element that an assistive app can access.

func setAccessibilityTraits(UIAccessibilityTraits)

Sets the combination of accessibility traits that best characterize the accessibility element.

func setAccessibilityImageRegions([WKAccessibilityImageRegion])

Marks portions of an image as separate accessible elements.

### Setting the Layout Direction

func setSemanticContentAttribute(WKInterfaceSemanticContentAttribute)

Sets the semantic description of the object’s contents, used to determine whether its content should be flipped when switching between left-to-right and right-to-left layouts.

### Constants

enum WKInterfaceObjectHorizontalAlignment

Constants for horizontally aligning objects in their container.

enum WKInterfaceObjectVerticalAlignment

Constants for vertically aligning objects in their container.

## Relationships

### Inherits From

- NSObject

### Inherited By

- WKInterfaceActivityRing
- WKInterfaceAuthorizationAppleIDButton
- WKInterfaceButton
- WKInterfaceDate
- WKInterfaceGroup
- WKInterfaceHMCamera
- WKInterfaceImage
- WKInterfaceInlineMovie
- WKInterfaceLabel
- WKInterfaceMap
- WKInterfaceMovie
- WKInterfacePaymentButton
- WKInterfacePicker
- WKInterfaceSCNScene
- WKInterfaceSKScene
- WKInterfaceSeparator
- WKInterfaceSlider
- WKInterfaceSwitch
- WKInterfaceTable
- WKInterfaceTextField
- WKInterfaceTimer
- WKInterfaceVolumeControl

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### User interface basics

Building watchOS app Interfaces Using the Storyboard

Create the user interface for your watchOS app by nesting stacks.

class WKInterfaceController

A class that provides the infrastructure for managing the interface in a watchOS app.

class WKAlertAction

An object that encapsulates information about a button displayed in an alert or action sheet.

class WKAccessibilityImageRegion

An object that defines a portion of an image that you want to call out separately to an assistive app.

func WKAccessibilityIsVoiceOverRunning() -> Bool

Returns a Boolean value indicating whether VoiceOver is running.

func WKAccessibilityIsReduceMotionEnabled() -> Bool

Returns a Boolean value indicating whether reduced motion is enabled.

