

- UIKit
-  UIContentUnavailableView 

Class

# UIContentUnavailableView

A view that indicates there’s no content to display.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UIContentUnavailableView
```

## Overview

Use a content-unavailable view to indicate that your app can’t display content. For example, content may not be available if a search returns no results or your app is loading data over the network.

In many cases, you won’t need to create a view of this type directly. Set a UIContentUnavailableConfiguration as the view controller’s contentUnavailableConfiguration, and the view controller manages the layout of the content-unavailable view.

## Topics

### Initializers

init(coder: NSCoder)

Creates a view from data in an unarchiver.

convenience init(configuration: UIContentUnavailableConfiguration)

Creates a new content-unavailable view with the specified configuration.

### Instance Properties

var isScrollEnabled: Bool

A Boolean value that determines whether the view content can scroll.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
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
- UIContentView
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

class UIImageView

A view that displays a single image or a sequence of animated images in your interface.

class UIPickerView

A view that uses a spinning-wheel or slot-machine metaphor to show one or more sets of values.

class UIProgressView

A view that depicts the progress of a task over time.

class UIWebView

A view that embeds web content in your app.

Deprecated

