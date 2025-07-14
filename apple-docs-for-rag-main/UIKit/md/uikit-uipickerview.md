

- UIKit
-  UIPickerView 

Class

# UIPickerView

A view that uses a spinning-wheel or slot-machine metaphor to show one or more sets of values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPickerView
```

## Overview

A picker view displays one or more wheels that the user manipulates to select items. Each wheel — known as a *component* — has a series of indexed rows representing the selectable items. Each row displays a string or view so that the user can identify the item on that row. Users select items by rotating the wheels to the desired values, which align with a selection indicator.

Note

The UIDatePicker class uses a custom subclass of UIPickerView to display dates and times. To see an example, tap the add (”+”) button in the Alarm pane of the Clock app.

You provide the data to display in your picker view using a picker data source (an object that adopts the UIPickerViewDataSource protocol). Use your picker view delegate (an object that adopts the UIPickerViewDelegate protocol) to provide views for displaying your data and responding to user selections.

Important

UIPickerView and its descendants aren’t available when the user interface idiom is UIUserInterfaceIdiom.mac.

## Topics

### Providing the picker data

var dataSource: (any UIPickerViewDataSource)?

The data source for the picker view.

protocol UIPickerViewDataSource

The interface for a picker view’s data source.

### Customizing the picker behavior

var delegate: (any UIPickerViewDelegate)?

The delegate for the picker view.

protocol UIPickerViewDelegate

The interface for a picker view’s delegate.

### Getting the dimensions of the picker view

var numberOfComponents: Int

The number of components for the picker view.

func numberOfRows(inComponent: Int) -> Int

Returns the number of rows for a component.

func rowSize(forComponent: Int) -> CGSize

Returns the size of a row for a component.

### Reloading the picker view

func reloadAllComponents()

Reloads all components of the picker view.

func reloadComponent(Int)

Reloads a particular component of the picker view.

### Selecting rows in the view picker

func selectRow(Int, inComponent: Int, animated: Bool)

Selects a row in a specified component of the picker view.

func selectedRow(inComponent: Int) -> Int

Returns the index of the selected row in a given component.

### Returning the view for a row and component

func view(forRow: Int, forComponent: Int) -> UIView?

Returns the view used by the picker view for a given row and component.

### Managing the appearance of the picker view

var showsSelectionIndicator: Bool

A Boolean value that determines whether the selection indicator is displayed.

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

class UIProgressView

A view that depicts the progress of a task over time.

class UIWebView

A view that embeds web content in your app.

Deprecated

