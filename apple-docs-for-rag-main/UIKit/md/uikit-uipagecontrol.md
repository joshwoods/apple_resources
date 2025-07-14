

- UIKit
-  UIPageControl 

Class

# UIPageControl

A control that displays a horizontal series of dots, each of which corresponds to a page in the app’s document or other data-model entity.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIPageControl
```

## Mentioned in 

Choosing a user interface idiom for your Mac app

Attaching gesture recognizers to UIKit controls

## Overview

For an example of a page control, see the Weather app when it’s configured to display information for more than one location.

When a user taps a page control to move to the next or previous page, the control sends the valueChanged event for handling by the delegate. The delegate can then evaluate the currentPage property to determine the page to display. The page control advances only one page in either direction. The currently viewed page is indicated by a white dot. Depending on the device, a certain number of dots are displayed on the screen before they’re clipped.

## Topics

### Managing pages

var currentPage: Int

The current page, shown by the page control as a white dot.

var numberOfPages: Int

The number of pages the receiver shows (as dots).

var hidesForSinglePage: Bool

A Boolean value that controls whether the page control is hidden when there is only one page.

var defersCurrentPageDisplay: Bool

A Boolean value that controls when the current page is displayed.

Deprecated

func updateCurrentPageDisplay()

Updates the page indicator to the current page.

Deprecated

### Coloring the page indicator

var pageIndicatorTintColor: UIColor?

The tint color to apply to the page indicator.

var currentPageIndicatorTintColor: UIColor?

The tint color to apply to the current page indicator.

### Managing the indicator images

var preferredIndicatorImage: UIImage?

The preferred image for indicators.

func indicatorImage(forPage: Int) -> UIImage?

Returns the override image for the indicator of the specified page.

func setIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the indicator of the specified page.

var preferredCurrentPageIndicatorImage: UIImage?

The preferred image for the current page indicator.

func currentPageIndicatorImage(forPage: Int) -> UIImage?

Returns the override image for the current page indicator of the specified page.

func setCurrentPageIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the current page indicator of the specified page.

### Customizing the layout direction

var direction: UIPageControl.Direction

The layout direction of the page indicators.

enum Direction

Decribes the layout direction of a page control’s indicators.

### Customizing the background style

var backgroundStyle: UIPageControl.BackgroundStyle

The preferred background style.

enum BackgroundStyle

Constants that define the background styles of the page control.

### Customizing the interaction state

var allowsContinuousInteraction: Bool

A Boolean value that determines whether the page control allows continuous interaction.

var interactionState: UIPageControl.InteractionState

The interaction state when the current page changes.

enum InteractionState

Constants that define the interaction states of the page control.

### Calculating the control size

func size(forNumberOfPages: Int) -> CGSize

Returns the size the receiver’s bounds should be to accommodate the given number of pages.

### Configuring page progress

var progress: UIPageControlProgress?

class UIPageControlProgress

class UIPageControlTimerProgress

protocol UIPageControlProgressDelegate

protocol UIPageControlTimerProgressDelegate

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

class UISegmentedControl

A horizontal control that consists of multiple segments, each segment functioning as a discrete button.

class UISlider

A control for selecting a single value from a continuous range of values.

class UIStepper

A control for incrementing or decrementing a value.

class UISwitch

A control that offers a binary choice, such as on/off.

