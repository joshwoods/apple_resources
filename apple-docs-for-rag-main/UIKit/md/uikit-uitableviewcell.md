

- UIKit
-  UITableViewCell 

Class

# UITableViewCell

The visual representation of a single row in a table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITableViewCell
```

## Mentioned in 

Filling a table with data

Configuring the cells for your table

Adding user-focusable elements to a tvOS app

## Overview

A UITableViewCell object is a specialized type of view that manages the content of a single table row. You use cells primarily to organize and present your app’s custom content, but UITableViewCell provides some specific customizations to support table-related behaviors, including:

- Applying a selection or highlight color to the cell

- Adding standard accessory views, such as a detail or disclosure control

- Putting the cell into an editable state

- Indenting the cell’s content to create a visual hierarchy in your table

Your app’s content occupies most of the cell’s bounds, but the cell may adjust that space to make room for other content. Cells display accessory views on the trailing edge of their content area. When you put your table into edit mode, the cell adds a delete control to the leading edge of its content area, and optionally swaps out an accessory view for a reorder control.

Every table view must have at least one type of cell for displaying content, and tables may have multiple cell types to display different types of content. Your table’s data source object handles the creation and configuration of cells immediately before they appear onscreen. For information about how to create your table’s cells, see Filling a table with data.

### Configure your cell’s content

Configure the content and layout of your cells in your storyboard file. Tables have one cell type by default, but you can add more by changing the value in the table’s Prototype Cells attribute. In addition to configuring the cell’s content, make sure you configure the following attributes:

- Identifier. Use this identifier (also known as a reuse identifier) to create the cell.

- Style. Choose one of the standard types or define a custom cell.

- Class. Specify a UITableViewCell subclass with your custom behavior.

To configure the content and appearance of your cell, you can set its contentConfiguration and backgroundConfiguration.

## Topics

### Creating a table view cell

init(style: UITableViewCell.CellStyle, reuseIdentifier: String?)

Initializes a table cell with a style and a reuse identifier and returns it to the caller.

enum CellStyle

An enumeration for the various styles of cells.

init?(coder: NSCoder)

Creates a table view from data in an unarchiver.

### Reusing cells

var reuseIdentifier: String?

A string for identifying a reusable cell.

func prepareForReuse()

Prepares a reusable cell for reuse by the table view’s delegate.

### Configuring the background

func defaultBackgroundConfiguration() -> UIBackgroundConfiguration

Retrieves a background configuration with system default values.

var backgroundConfiguration: UIBackgroundConfiguration?

The current background configuration of the cell.

var automaticallyUpdatesBackgroundConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its background configuration when its state changes.

var backgroundView: UIView?

The view to use as the background of the cell.

var selectedBackgroundView: UIView?

The view to use as the background for a selected cell.

var multipleSelectionBackgroundView: UIView?

The background view to use for a selected cell when the table view allows multiple row selections.

### Managing the content

func defaultContentConfiguration() -> UIListContentConfiguration

Retrieves a default list content configuration for the cell’s style.

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the cell.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its content configuration when its state changes.

var contentView: UIView

The content view of the cell object.

### Managing the state

var configurationState: UICellConfigurationState

The current configuration state of the cell.

func setNeedsUpdateConfiguration()

Informs the cell to update its configuration for its current state.

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

var configurationUpdateHandler: UITableViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

typealias ConfigurationUpdateHandler

The type of block for handling updates to the cell’s configuration using the current state.

### Managing accessory views

var accessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s normal state.

var accessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s normal state.

var editingAccessoryType: UITableViewCell.AccessoryType

The type of standard accessory view for the cell to use in the table view’s editing state.

var editingAccessoryView: UIView?

The view to use on the right side of the cell, typically as a control, in the table view’s editing state.

enum AccessoryType

The type of standard accessory control used by a cell.

### Managing cell selection and highlighting

var selectionStyle: UITableViewCell.SelectionStyle

The style of selection for a cell.

enum SelectionStyle

The style of selected cells.

var isSelected: Bool

A Boolean value that indicates whether the cell is selected.

func setSelected(Bool, animated: Bool)

Sets the selected state of the cell, optionally animating the transition between states.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is highlighted.

func setHighlighted(Bool, animated: Bool)

Sets the highlighted state of the cell, optionally animating the transition between states.

### Editing the cell

var isEditing: Bool

A Boolean value that indicates whether the cell is in an editable state.

func setEditing(Bool, animated: Bool)

Toggles the cell into and out of editing mode.

var editingStyle: UITableViewCell.EditingStyle

The editing style of the cell.

enum EditingStyle

The editing control used by a cell.

var showingDeleteConfirmation: Bool

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

var showsReorderControl: Bool

A Boolean value that determines whether the cell shows the reordering control.

### Dragging the row

var userInteractionEnabledWhileDragging: Bool

A Boolean value indicating whether users can interact with a cell while it is being dragged.

func dragStateDidChange(UITableViewCell.DragState)

Notifies the cell that its drag status changed.

enum DragState

Constants indicating the current state of a row involved in a drag operation.

### Adjusting to state transitions

func willTransition(to: UITableViewCell.StateMask)

Notifies the cell that it’s about to transition to a new cell state.

func didTransition(to: UITableViewCell.StateMask)

Notifies the cell that it transitioned to a new cell state.

struct StateMask

Constants used to determine the new state of a cell as it transitions between states.

### Managing content indentation

var indentationLevel: Int

The indentation level of the cell’s content.

var indentationWidth: CGFloat

The width for each level of indentation of a cell’s content.

var shouldIndentWhileEditing: Bool

A Boolean value that controls whether the cell background is indented when the table view is in editing mode.

var separatorInset: UIEdgeInsets

The inset values for the separator line drawn beneath the cell.

enum SeparatorStyle

The style for cells to use as separators.

### Managing focus

var focusStyle: UITableViewCell.FocusStyle

The appearance of the cell when focused.

enum FocusStyle

The style of focused cells.

### Deprecated

var textLabel: UILabel?

The label to use for the main textual content of the table cell.

Deprecated

var detailTextLabel: UILabel?

The secondary label of the table cell, if one exists.

Deprecated

var imageView: UIImageView?

The image view of the table cell.

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
- UIGestureRecognizerDelegate
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

class UITableViewHeaderFooterView

A reusable view that you place at the top or bottom of a table section to display additional information for that section.

