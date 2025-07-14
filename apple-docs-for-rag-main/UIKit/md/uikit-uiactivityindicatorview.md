

- UIKit
-  UIActivityIndicatorView 

Class

# UIActivityIndicatorView

A view that shows that a task is in progress.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIActivityIndicatorView
```

## Overview

You control when an activity indicator animates by calling the startAnimating() and stopAnimating() methods. To automatically hide the activity indicator when animation stops, set the hidesWhenStopped property to true.

You can set the color of the activity indicator by using the color property.

## Topics

### Creating an activity indicator

init(style: UIActivityIndicatorView.Style)

Creates an activity indicator.

init(frame: CGRect)

Creates an activity indicator with the specified frame rectangle.

init(coder: NSCoder)

Creates an activity indicator from data in an unarchiver.

### Managing an activity indicator

func startAnimating()

Starts the animation of the progress indicator.

func stopAnimating()

Stops the animation of the progress indicator.

var isAnimating: Bool

A Boolean value indicating whether the activity indicator is currently running its animation.

var hidesWhenStopped: Bool

A Boolean value that controls whether the activity indicator is hidden when the animation is stopped.

### Configuring the activity indicator appearance

var style: UIActivityIndicatorView.Style

The basic appearance of the activity indicator.

var color: UIColor!

The color of the activity indicator.

### Constants

enum Style

The visual style of the progress indicator.

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
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Content views

class UICalendarView

A view that displays a calendar with date-specific decorations, and provides for user selection of a single date or multiple dates.

class UIContentUnavailableView

A view that indicates there’s no content to display.

class UIImageView

A view that displays a single image or a sequence of animated images in your interface.

class UIPickerView

A view that uses a spinning-wheel or slot-machine metaphor to show one or more sets of values.

class UIProgressView

A view that depicts the progress of a task over time.

class UIWebView

A view that embeds web content in your app.

Deprecated

