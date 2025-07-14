

- UIKit
-  UIPopoverBackgroundView 

Class

# UIPopoverBackgroundView

The background appearance for a popover.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIPopoverBackgroundView
```

## Overview

This class must be subclassed before it can be used. The implementation of your subclass is responsible for providing the border decoration and arrow for the popover. Subclasses must override all declared properties and methods to provide information about where to lay out the corresponding popover content and arrow. Subclasses must also provide implementations for all methods of the UIPopoverBackgroundViewMethods protocol.

### Subclassing notes

Your subclass is responsible for providing the background visual styling of the popover, which includes the arrow and appropriately styled border. The popover controller places the actual popover content on top of your background view to finish the popover’s presentation.

The background contents of your view should be based on stretchable images. Because the popover is animated into place (and may require animated transitions), using images is the only way to ensure that the animations are smooth and not jittery. By creating images that can be stretched at appropriate places, your popover can still be resized and adjusted as needed. You can then incorporate those images using UIImageView subviews or Core Animation layers. When the size of the popover changes (perhaps to accommodate the keyboard), all you have to do is adjust the frame rectangles of your embedded image views.

Note

The images you use for your popover background view shouldn’t contain any shadow effects. The popover controller adds a shadow to the popover for you.

In addition to providing the background content, your subclass must implement the arrowOffset and arrowDirection properties and the methods in the UIPopoverBackgroundViewMethods protocol. The popover controller uses these methods and properties to get and set information related to your background view. The protocol methods are called once and the values you return should never change. However, the values in the arrowOffset and arrowDirection properties can change while your popover is on the screen, so your setter methods should call setNeedsLayout() when that happens to update the background image views or layers.

To create a stretchable image, use the resizableImage(withCapInsets:) method of UIImage.

## Topics

### Accessing the arrow metrics

var arrowOffset: CGFloat

The distance (measured in points) from the center of the view to the center line of the arrow.

var arrowDirection: UIPopoverArrowDirection

The direction in which the popover arrow is pointing.

### Controlling the popover appearance

class var wantsDefaultContentAppearance: Bool

Determines whether the default content appearance should be used for the popover.

Deprecated

## Relationships

### Inherits From

- UIView

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
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverBackgroundViewMethods
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Popovers

Displaying transient content in a popover

Show a temporary interface on top of your app’s content on iPad.

class UIPopoverPresentationController

An object that manages the display of content in a popover.

protocol UIPopoverBackgroundViewMethods

A set of methods that popover background view subclasses must implement.

