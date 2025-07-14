

- Notification Center
-  NCWidgetListViewController Deprecated

Class

# NCWidgetListViewController

An object that provides a list view for displaying content in a macOS Today widget.

macOS 10.10–11.0Deprecated

``` source
@MainActor
class NCWidgetListViewController
```

Deprecated

Use WidgetKit instead.

## Overview

The `NCWidgetListViewController` class provides a list view for displaying content in a Today widget. A list view controller works together with its delegate to display content and support user interaction with the list. To learn about the list view controller delegate methods, see NCWidgetListViewDelegate.

You store the contents of a widget as an array of objects in the list view controller’s contents property. To display the objects, you use a delegate object, which provides a custom view controller for each object in `contents`. A list view controller also provides properties that make it easy to specify aspects of the list’s appearance and behavior, such as the number of rows to display, the presence of divider lines, and the ability to edit the list.

## Topics

### Displaying and Editing List Content

var delegate: (any NCWidgetListViewDelegate)?

The list view controller’s delegate or `nil` if the receiver doesn’t have a delegate.

protocol NCWidgetListViewDelegate

The interface for handling content display and editing in the list view of a macOS Today widget.

### Accessing Content

var contents: [Any]

An array of objects to display in the list view.

func row(for: NSViewController) -> Int

Returns the row represented by the specified content view controller.

func viewController(atRow: Int, makeIfNecessary: Bool) -> NSViewController

Returns the content view controller associated with the specified row, or a new content view controller if desired.

### Customizing the List Appearance

var minimumVisibleRowCount: Int

The minimum number of visible rows to display.

var hasDividerLines: Bool

A Boolean value that indicates whether list displays divider lines between rows.

### Supporting Editing

var editing: Bool

A Boolean value that indicates whether the list is in editing mode.

var showsAddButtonWhenEditing: Bool

A Boolean value that indicates whether an Add (+) button is displayed while the list is in editing mode.

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

