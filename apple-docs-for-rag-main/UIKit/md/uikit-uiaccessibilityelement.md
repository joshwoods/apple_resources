

- UIKit
-  UIAccessibilityElement 

Class

# UIAccessibilityElement

An element that should be accessible to users with disabilities, but that isn’t accessible by default.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIAccessibilityElement
```

## Mentioned in 

Supporting VoiceOver in your app

## Overview

You can use UIAccessibilityElement to provide information about an icon or text image that isn’t automatically accessible because it doesn’t inherit from UIView (or UIControl). A view that contains such nonview items creates an instance of UIAccessibilityElement to represent each item that needs to be accessible.

The properties of an accessibility element provide information about the element, such as location and current value, to an assistive application. You might need to set an element’s property even if you don’t need to create an instance of `UIAccessibilityElement` to represent it. For example, if your app includes a button with a custom icon that means “solve,” the button itself is already represented by an accessibility element because it’s a subclass of UIButton. However, you need to supply information for the label and hint properties because this information is unique to this button. You can do this in Interface Builder or by setting the properties in the UIAccessibility informal protocol.

## Topics

### Creating an accessibility element

init(accessibilityContainer: Any)

Creates and initializes an accessibility element to represent an item in the specified container.

### Accessing the containing view

var accessibilityContainer: AnyObject?

The view that contains the accessibility element.

### Determining accessibility

var isAccessibilityElement: Bool

A Boolean value indicating whether the item is an accessibility element an assistive application can access.

### Accessing the attributes of an accessibility element

var accessibilityLabel: String?

A string that succinctly identifies the accessibility element.

var accessibilityHint: String?

A string that briefly describes the result of performing an action on the accessibility element.

var accessibilityValue: String?

A string that represents the current value of the accessibility element.

var accessibilityFrame: CGRect

The frame of the accessibility element, in screen coordinates.

var accessibilityFrameInContainerSpace: CGRect

The frame of the accessibility element, in the coordinate space of its container view.

var accessibilityTraits: UIAccessibilityTraits

The combination of traits that best characterize the accessibility element.

## Relationships

### Inherits From

- UIResponder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTouchBarProvider
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Elements

protocol UIScrollViewAccessibilityDelegate

A set of methods you can implement to provide accessibility information for a scroll view.

protocol UIPickerViewAccessibilityDelegate

A set of methods you can implement to provide accessibility information for individual components of a picker view.

