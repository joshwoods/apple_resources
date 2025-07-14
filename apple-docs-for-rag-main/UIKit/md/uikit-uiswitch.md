

- UIKit
-  UISwitch 

Class

# UISwitch

A control that offers a binary choice, such as on/off.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UISwitch
```

## Mentioned in 

Attaching gesture recognizers to UIKit controls

Displaying a checkbox in your Mac app built with Mac Catalyst

Choosing a user interface idiom for your Mac app

## Overview

The UISwitch class declares a property and a method to control its on/off state. When a person manipulates the switch control (“flips” it), it triggers the valueChanged event.

You can customize the appearance of the switch by changing the color used to tint the switch when it’s on or off.

For information about basic view behaviors, see View Programming Guide for iOS.

## Topics

### Creating a switch

init(frame: CGRect)

Creates a switch control.

init?(coder: NSCoder)

Creates a switch control from data in an unarchiver.

### Setting the on/off state

var isOn: Bool

A Boolean value that determines whether the switch is in the on or off position.

func setOn(Bool, animated: Bool)

Sets the state of the switch to the on or off position, optionally animating the transition.

### Setting the display style

Displaying a checkbox in your Mac app built with Mac Catalyst

Present a switch control as a Mac-style checkbox when your app runs in the Mac user interface idiom.

var preferredStyle: UISwitch.Style

The preferred display style for the switch.

var style: UISwitch.Style

The display style for the switch.

enum Style

Styles that determine the appearance of the switch.

var title: String?

The title displayed next to a checkbox-style switch.

### Customizing the appearance of the switch

var onTintColor: UIColor?

The color used to tint the appearance of the switch when it’s in the on position.

var thumbTintColor: UIColor?

The color used to tint the appearance of the thumb.

### Deprecated

var onImage: UIImage?

The image displayed when the switch is in the on position.

var offImage: UIImage?

The image displayed when the switch is in the off position.

## Relationships

### Inherits From

- UIControl

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Controls

Responding to control-based events using target-action

Handle user input by connecting buttons, sliders, and other controls to your app’s code using the target-action design pattern.

class UIControl

The base class for controls, which are visual elements that convey a specific action or intention in response to user interactions.

class UIButton

A control that executes your custom code in response to user interactions.

class UIColorWell

A control that displays a color picker.

class UIDatePicker

A control for inputting date and time values.

class UIPageControl

A control that displays a horizontal series of dots, each of which corresponds to a page in the app’s document or other data-model entity.

class UISegmentedControl

A horizontal control that consists of multiple segments, each segment functioning as a discrete button.

class UISlider

A control for selecting a single value from a continuous range of values.

class UIStepper

A control for incrementing or decrementing a value.

