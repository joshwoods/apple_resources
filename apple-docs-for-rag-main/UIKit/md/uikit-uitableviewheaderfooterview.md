

- UIKit
-  UITableViewHeaderFooterView 

Class

# UITableViewHeaderFooterView

A reusable view that you place at the top or bottom of a table section to display additional information for that section.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITableViewHeaderFooterView
```

## Mentioned in 

Adding headers and footers to table sections

## Overview

Use UITableViewHeaderFooterView objects to manage the header and footer content of your table’s sections efficiently. A header-footer view is a reusable view that you can subclass or use as is. To configure the content and appearance of a header-footer view, you can set its contentConfiguration and backgroundConfiguration.

To promote the reuse of your header-footer views, register them by calling the register(_:forHeaderFooterViewReuseIdentifier:) or register(_:forHeaderFooterViewReuseIdentifier:) method of the table view. In the tableView(_:viewForHeaderInSection:) or tableView(_:viewForFooterInSection:) method of your delegate object, call the table view’s dequeueReusableHeaderFooterView(withIdentifier:) method to create your view. That method returns a recycled view (if one is available) or creates a new view using the information you registered.

A simple alternative to creating custom header-footer views is to implement the tableView(_:titleForHeaderInSection:) and tableView(_:titleForFooterInSection:) methods of your data source object. When you implement those methods, the table view creates a standard header or footer view and displays the text you supply.

## Topics

### Creating the view

init(reuseIdentifier: String?)

Initializes a header-footer view with the specified reuse identifier.

init?(coder: NSCoder)

Creates a header-footer view from data in an unarchiver.

### Managing view reuse

var reuseIdentifier: String?

A string used to identify a reusable header or footer.

func prepareForReuse()

Prepares a reusable header or footer view for reuse by the table.

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the view.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the view automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The background view of the header or footer.

### Managing the content

func defaultContentConfiguration() -> UIListContentConfiguration

Retrieves a default list content configuration for the view’s style.

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the view.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the view automatically updates its content configuration when its state changes.

var contentView: UIView

The content view of the header or footer.

### Managing the state

var configurationState: UIViewConfigurationState

The current configuration state of the view.

func setNeedsUpdateConfiguration()

Informs the view to update its configuration for its current state.

func updateConfiguration(using: UIViewConfigurationState)

Updates the view’s configuration using the current state.

var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler?

A block for handling updates to the view’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the view’s configuration using the current state.

### Deprecated

var textLabel: UILabel?

A primary text label for the view.

Deprecated

var detailTextLabel: UILabel?

A detail text label for the view.

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

### Cells, headers, and footers

Configuring the cells for your table

Specify the appearance and content of your table’s rows by defining one or more prototype cells in your storyboard.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

Adding headers and footers to table sections

Differentiate groups of rows visually by adding header and footer views to your table view’s sections.

class UITableViewCell

The visual representation of a single row in a table view.

