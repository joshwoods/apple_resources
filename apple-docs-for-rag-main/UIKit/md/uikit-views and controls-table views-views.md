

- UIKit
- Views and controls
-  Table views 

API Collection

# Table views

Display data in a single column of customizable rows.

## Overview

A table view displays a single column of vertically scrolling content, divided into rows and sections. Each row of a table displays a single piece of information related to your app. Sections let you group related rows together. For example, the Contacts app uses a table to display the names of the user’s contacts.

Table views are a collaboration between many different objects, including:

- Cells. A cell provides the visual representation for your content. You can use the default cells provided by UIKit or define custom cells to suit the needs of your app.

- Table view controller. You typically use a UITableViewController object to manage a table view. You can use other view controllers too, but a table view controller is required for some table-related features to work.

- Your data source object. This object adopts the UITableViewDataSource protocol and provides the data for the table.

- Your delegate object. This object adopts the UITableViewDelegate protocol and manages user interactions with the table’s contents.

## Topics

### Essentials

class UITableView

A view that presents data using rows in a single column.

### Data

Filling a table with data

Create and configure cells for your table dynamically using a data source object, or provide them statically from your storyboard.

Asynchronously loading images into table and collection views

Store and fetch images asynchronously to make your app more responsive.

protocol UITableViewDataSource

The methods that an object adopts to manage data and provide cells for a table view.

protocol UITableViewDataSourcePrefetching

A protocol that provides advance warning of the data requirements for a table view, allowing you to start potentially long-running data operations early.

class UITableViewDiffableDataSource

The object you use to manage data and provide cells for a table view.

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

class UILocalizedIndexedCollation

An object that organizes, sorts, and localizes the data for a table view that has a section index.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

### Table management

Estimating the height of a table’s scrolling area

Provide height estimates for your table view’s headers, footers, and rows to ensure that scrolling accurately reflects the size of your content.

class UITableViewController

A view controller that specializes in managing a table view.

protocol UITableViewDelegate

Methods for managing selections, configuring section headers and footers, deleting and reordering cells, and performing other actions in a table view.

class UITableViewFocusUpdateContext

A context object that provides information relevant to a specific focus update from one view to another.

### Cells, headers, and footers

Configuring the cells for your table

Specify the appearance and content of your table’s rows by defining one or more prototype cells in your storyboard.

Creating self-sizing table view cells

Create table view cells that support Dynamic Type and use system spacing constraints to adjust the spacing surrounding text labels.

Adding headers and footers to table sections

Differentiate groups of rows visually by adding header and footer views to your table view’s sections.

class UITableViewCell

The visual representation of a single row in a table view.

class UITableViewHeaderFooterView

A reusable view that you place at the top or bottom of a table section to display additional information for that section.

### Row actions

class UISwipeActionsConfiguration

The set of actions to perform when swiping on rows of a table.

class UIContextualAction

An action to display when the user swipes a table row.

class UITableViewRowAction

A single action to present when the user swipes horizontally in a table row.

Deprecated

### Selection management

Handling row selection in a table view

Detect when a user taps a table view cell so your app can take the next indicated action.

Selecting multiple items with a two-finger pan gesture

Accelerate user selection of multiple items using the multiselect gesture on table and collection views.

### Drag and drop

Supporting drag and drop in table views

Initiate drags and handle drops from a table view.

Adopting drag and drop in a table view

Demonstrates how to enable and implement drag and drop for a table view.

protocol UITableViewDragDelegate

The interface for initiating drags from a table view.

protocol UITableViewDropDelegate

The interface for handling drops in a table view.

protocol UITableViewDropCoordinator

An interface for coordinating your custom drop-related actions with the table view.

protocol UITableViewDropItem

The data associated with an item being dropped into the table view.

class UITableViewDropProposal

Your proposed solution for handling a drop in a table view.

### Placeholder cells

protocol UITableViewDropPlaceholderContext

An object for tracking a placeholder cell that you added to your table during a drop operation.

class UITableViewDropPlaceholder

A placeholder cell that supports customizing the drop preview parameters.

class UITableViewPlaceholder

An object that contains information about a placeholder cell being inserted into a table.

## See Also

### Container views

Autosizing Views for Localization in iOS

Add auto layout constraints to your app to achieve localizable views.

Collection views

Display nested views using a configurable and highly customizable layout.

class UIStackView

A streamlined interface for laying out a collection of views in either a column or a row.

class UIScrollView

A view that allows the scrolling and zooming of its contained views.

