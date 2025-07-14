

- UIKit
-  UIProgressView 

Class

# UIProgressView

A view that depicts the progress of a task over time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIProgressView
```

## Overview

The UIProgressView class provides properties for managing the style of the progress bar and for getting and setting values that are pinned to the progress of a task.

For an indeterminate progress indicator — or a “spinner” — use an instance of the UIActivityIndicatorView class.

## Topics

### Creating a progress view

convenience init(progressViewStyle: UIProgressView.Style)

Creates a progress view with the specified style.

init(frame: CGRect)

Creates a progress view with the specified frame rectangle.

init?(coder: NSCoder)

Creates a progress view from data in an unarchiver.

### Managing the progress bar

var progress: Float

The current progress of the progress view.

func setProgress(Float, animated: Bool)

Adjusts the current progress of the progress view, optionally animating the change.

var observedProgress: Progress?

The progress object to use for updating the progress view.

### Configuring the progress bar

var progressViewStyle: UIProgressView.Style

The current graphical style of the progress view.

var progressTintColor: UIColor?

The color shown for the portion of the progress bar that’s filled.

var progressImage: UIImage?

An image to use for the portion of the progress bar that’s filled.

var trackTintColor: UIColor?

The color shown for the portion of the progress bar that isn’t filled.

var trackImage: UIImage?

An image to use for the portion of the track that isn’t filled.

### Constants

enum Style

The styles permitted for the progress bar.

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

class UIActivityIndicatorView

A view that shows that a task is in progress.

class UICalendarView

A view that displays a calendar with date-specific decorations, and provides for user selection of a single date or multiple dates.

class UIContentUnavailableView

A view that indicates there’s no content to display.

class UIImageView

A view that displays a single image or a sequence of animated images in your interface.

class UIPickerView

A view that uses a spinning-wheel or slot-machine metaphor to show one or more sets of values.

class UIWebView

A view that embeds web content in your app.

Deprecated

