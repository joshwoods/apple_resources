

- UIKit
-  UITableView 

Class

# UITableView

A view that presents data using rows in a single column.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UITableView
```

## Mentioned in 

Configuring the cells for your table

Adding headers and footers to table sections

Making a view into a drop destination

Making a view into a drag source

Estimating the height of a table’s scrolling area

## Overview

Table views in iOS display rows of vertically scrolling content in a single column. Each row in the table contains one piece of your app’s content. For example, the Contacts app displays the name of each contact in a separate row, and the main page of the Settings app displays the available groups of settings. You can configure a table to display a single long list of rows, or you can group related rows into sections to make navigating the content easier.

Tables are common in apps with data that’s highly structured or organized hierarchically. Apps that contain hierarchical data often use tables in conjunction with a navigation view controller, which facilitates navigation between different levels of the hierarchy. For example, the Settings app uses tables and a navigation controller to organize the system settings.

UITableView manages the basic appearance of the table, but your app provides the cells (UITableViewCell objects) that display the actual content. The standard cell configurations display a simple combination of text and images, but you can define custom cells that display any content you want. You can also supply header and footer views to provide additional information for groups of cells.

### Add a table view to your interface

To add a table view to your interface, drag a table view controller (UITableViewController) object to your storyboard. Xcode creates a new scene that includes both the view controller and a table view, ready for you to configure and use.

Table views are data-driven, normally getting their data from a data source object that you provide. The data source object manages your app’s data and is responsible for creating and configuring the table’s cells. If the content of your table never changes, you can configure that content in your storyboard file instead.

For information about how to specify your table’s data, see Filling a table with data.

### Save and restore the table’s current state

Table views support UIKit app restoration. To save and restore the table’s data, assign a nonempty value to the table view’s restorationIdentifier property. When you save its parent view controller, the table view automatically saves the index paths for the currently selected and visible rows. If the table’s data source object adopts the UIDataSourceModelAssociation protocol, the table stores the unique IDs that you provide for those items instead of their index paths.

For information about how to save and restore your app’s state information, see Preserving your app’s UI across launches.

## Topics

### Creating a table view

init(frame: CGRect, style: UITableView.Style)

Creates and returns a table view with the specified frame and style.

init?(coder: NSCoder)

Creates a table view object from data in an unarchiver.

### Providing the data and cells

var dataSource: (any UITableViewDataSource)?

The object that acts as the data source of the table view.

var prefetchDataSource: (any UITableViewDataSourcePrefetching)?

The object that acts as the prefetching data source for the table view, receiving notifications of upcoming cell data requirements.

var isPrefetchingEnabled: Bool

A Boolean value that indicates whether to allow cell and data prefetching.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

### Recycling table view cells

func register(UINib?, forCellReuseIdentifier: String)

Registers a nib object that contains a cell with the table view under a specified identifier.

func register(AnyClass?, forCellReuseIdentifier: String)

Registers a class to use in creating new table cells.

func dequeueReusableCell(withIdentifier: String, for: IndexPath) -> UITableViewCell

Returns a reusable table-view cell object for the specified reuse identifier and adds it to the table.

func dequeueReusableCell(withIdentifier: String) -> UITableViewCell?

Returns a reusable table-view cell object after locating it by its identifier.

### Recycling section headers and footers

func register(UINib?, forHeaderFooterViewReuseIdentifier: String)

Registers a nib object that contains a header or footer with the table view under a specified identifier.

func register(AnyClass?, forHeaderFooterViewReuseIdentifier: String)

Registers a class to use in creating new table header or footer views.

func dequeueReusableHeaderFooterView(withIdentifier: String) -> UITableViewHeaderFooterView?

Returns a reusable header or footer view after locating it by its identifier.

### Managing interactions with the table

var delegate: (any UITableViewDelegate)?

The object that acts as the delegate of the table view.

protocol UITableViewDelegate

Methods for managing selections, configuring section headers and footers, deleting and reordering cells, and performing other actions in a table view.

### Configuring the table’s appearance

var style: UITableView.Style

The style of the table view.

enum Style

Constants for the table view styles.

var tableHeaderView: UIView?

The view that displays above the table’s content.

var tableFooterView: UIView?

The view that displays below the table’s content.

var backgroundView: UIView?

The background view of the table view.

### Configuring cell height and layout

var rowHeight: CGFloat

The default height in points of each row in the table view.

var estimatedRowHeight: CGFloat

The estimated height of rows in the table view.

var fillerRowHeight: CGFloat

The height for empty rows that fill the table view.

var cellLayoutMarginsFollowReadableWidth: Bool

A Boolean value that indicates whether the cell margins derive from the width of the readable content guide.

var insetsContentViewsToSafeArea: Bool

A Boolean value that indicates whether the table view adjusts the content views of its cells, headers, and footers to fit within the safe area.

### Configuring header and footer appearance

var sectionHeaderHeight: CGFloat

The height of section headers in the table view.

var sectionFooterHeight: CGFloat

The height of section footers in the table view.

var estimatedSectionHeaderHeight: CGFloat

The estimated height of section headers in the table view.

var estimatedSectionFooterHeight: CGFloat

The estimated height of section footers in the table view.

var sectionHeaderTopPadding: CGFloat

The amount of padding above each section header.

### Customizing the separator appearance

var separatorStyle: UITableViewCell.SeparatorStyle

The style for table cells to use as separators.

enum SeparatorStyle

The style for cells to use as separators.

var separatorColor: UIColor?

The color of separator rows in the table view.

var separatorEffect: UIVisualEffect?

The effect to apply to table separators.

var separatorInset: UIEdgeInsets

The default inset of cell separators.

var separatorInsetReference: UITableView.SeparatorInsetReference

An indicator of how to interpret the separator inset value.

enum SeparatorInsetReference

Constants that indicate how to interpret the separator inset value of a table view.

### Getting the number of rows and sections

func numberOfRows(inSection: Int) -> Int

Returns the number of rows (table cells) in a specified section.

var numberOfSections: Int

The number of sections in the table view.

### Getting cells and section-based views

func cellForRow(at: IndexPath) -> UITableViewCell?

Returns the table cell at the index path you specify.

func headerView(forSection: Int) -> UITableViewHeaderFooterView?

Returns the header view for the specified section.

func footerView(forSection: Int) -> UITableViewHeaderFooterView?

Returns the footer view for the specified section.

func indexPath(for: UITableViewCell) -> IndexPath?

Returns an index path that represents the row and section of a specified table-view cell.

func indexPathForRow(at: CGPoint) -> IndexPath?

Returns an index path that identifies the row and section at the specified point.

func indexPathsForRows(in: CGRect) -> [IndexPath]?

Returns an array of index paths, each representing a row that the specified rectangle encloses.

var visibleCells: [UITableViewCell]

The table cells that are visible in the table view.

var indexPathsForVisibleRows: [IndexPath]?

An array of index paths, each identifying a visible row in the table view.

### Selecting rows

var indexPathForSelectedRow: IndexPath?

An index path that identifies the row and section of the selected row.

var indexPathsForSelectedRows: [IndexPath]?

The index paths that represent the selected rows.

func selectRow(at: IndexPath?, animated: Bool, scrollPosition: UITableView.ScrollPosition)

Selects a row in the table view that an index path identifies, optionally scrolling the row to a location in the table view.

func deselectRow(at: IndexPath, animated: Bool)

Deselects a row that an index path identifies, with an option to animate the deselection.

var allowsSelection: Bool

A Boolean value that determines whether users can select a row.

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one row outside of editing mode.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the table view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

class let selectionDidChangeNotification: NSNotification.Name

A notification that posts when the selected row in the posting table view changes.

### Inserting, deleting, and moving rows and sections

func insertRows(at: [IndexPath], with: UITableView.RowAnimation)

Inserts rows in the table view at the locations that an array of index paths identifies, with an option to animate the insertion.

func deleteRows(at: [IndexPath], with: UITableView.RowAnimation)

Deletes the rows that an array of index paths identifies, with an option to animate the deletion.

func insertSections(IndexSet, with: UITableView.RowAnimation)

Inserts one or more sections in the table view, with an option to animate the insertion.

func deleteSections(IndexSet, with: UITableView.RowAnimation)

Deletes one or more sections in the table view, with an option to animate the deletion.

enum RowAnimation

The type of animation to use when inserting or deleting rows.

func moveRow(at: IndexPath, to: IndexPath)

Moves the row at a specified location to a destination location.

func moveSection(Int, toSection: Int)

Moves a section to a new location in the table view.

### Performing batch updates to rows and sections

func performBatchUpdates((() -> Void)?, completion: ((Bool) -> Void)?)

Animates multiple insert, delete, reload, and move operations as a group.

func beginUpdates()

Begins a series of method calls that insert, delete, or select rows and sections of the table view.

func endUpdates()

Concludes a series of method calls that insert, delete, select, or reload rows and sections of the table view.

### Reloading the table view

var hasUncommittedUpdates: Bool

A Boolean value that indicates whether the table view’s appearance contains changes that aren’t present in its data source.

func reconfigureRows(at: [IndexPath])

Updates the data for the rows at the index paths you specify, preserving the existing cells for the rows.

func reloadData()

Reloads the rows and sections of the table view.

func reloadRows(at: [IndexPath], with: UITableView.RowAnimation)

Reloads the specified rows using the provided animation effect.

func reloadSections(IndexSet, with: UITableView.RowAnimation)

Reloads the specified sections using the provided animation effect.

func reloadSectionIndexTitles()

Reloads the items in the index bar along the right side of the table view.

### Managing drag interactions

var dragDelegate: (any UITableViewDragDelegate)?

The delegate object that manages the dragging of items from the table view.

protocol UITableViewDragDelegate

The interface for initiating drags from a table view.

var hasActiveDrag: Bool

A Boolean value that indicates whether the table view is currently tracking a drag session.

var dragInteractionEnabled: Bool

A Boolean value that indicates whether the table view supports dragging content.

### Managing drop interactions

var dropDelegate: (any UITableViewDropDelegate)?

The delegate object that manages the dropping of content into the table view.

protocol UITableViewDropDelegate

The interface for handling drops in a table view.

var hasActiveDrop: Bool

A Boolean value that indicates whether the table view is currently tracking a drop session.

### Scrolling the table view

func scrollToRow(at: IndexPath, at: UITableView.ScrollPosition, animated: Bool)

Scrolls through the table view until a row that an index path identifies is at a particular location on the screen.

func scrollToNearestSelectedRow(at: UITableView.ScrollPosition, animated: Bool)

Scrolls the table view so that the selected row nearest to a specified position in the table view is at that position.

enum ScrollPosition

The position in the table view (top, middle, bottom) to scroll a specified row to.

### Putting the table into edit mode

func setEditing(Bool, animated: Bool)

Toggles the table view into and out of editing mode.

var isEditing: Bool

A Boolean value that determines whether the table view is in editing mode.

### Configuring the table index

var sectionIndexMinimumDisplayRowCount: Int

The number of table rows at which to display the index list on the right edge of the table.

var sectionIndexColor: UIColor?

The color to use for the table view’s index text.

var sectionIndexBackgroundColor: UIColor?

The color to use for the background of the table view’s section index.

var sectionIndexTrackingBackgroundColor: UIColor?

The color to use for the table view’s index background area.

class let indexSearch: String

A constant for adding the magnifying glass icon to the section index of a table view.

### Getting the drawing areas for the table

func rect(forSection: Int) -> CGRect

Returns the drawing area for a specified section of the table view.

func rectForRow(at: IndexPath) -> CGRect

Returns the drawing area for a row that an index path identifies.

func rectForFooter(inSection: Int) -> CGRect

Returns the drawing area for the footer of the specified section.

func rectForHeader(inSection: Int) -> CGRect

Returns the drawing area for the header of the specified section.

### Working with focus

var allowsFocus: Bool

A Boolean value that determines whether the table view allows its cells to become focused.

var allowsFocusDuringEditing: Bool

A Boolean value that determines whether the table view allows its cells to become focused in edit mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

var remembersLastFocusedIndexPath: Bool

A Boolean value that indicates whether the table view automatically returns the focus to the cell at the last focused index path.

### Managing context menus

var contextMenuInteraction: UIContextMenuInteraction?

The table view’s context menu interaction.

### Resizing self-sizing cells

var selfSizingInvalidation: UITableView.SelfSizingInvalidation

The mode that the table view uses for invalidating the size of self-sizing cells.

enum SelfSizingInvalidation

Constants that describe modes for invalidating the size of self-sizing table view cells.

### Managing content-hugging behavior

var contentHuggingElements: UITableViewContentHuggingElements

A setting that determines which type of items tightly hug their content.

struct UITableViewContentHuggingElements

Constants that determine which types of items in a table view tightly hug their content.

## Relationships

### Inherits From

- UIScrollView

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
- UICoordinateSpace
- UIDataSourceTranslating
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIFocusItemScrollableContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UISpringLoadedInteractionSupporting
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

