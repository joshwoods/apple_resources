

- UIKit
-  UITableViewDropDelegate 

Protocol

# UITableViewDropDelegate

The interface for handling drops in a table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITableViewDropDelegate : NSObjectProtocol
```

## Mentioned in 

Supporting drag and drop in table views

## Overview

Implement this protocol in the object that you use to incorporate dropped data into your table view. The only required method of this protocol is the tableView(_:performDropWith:) method, but you can implement other methods as needed to customize the drop behavior of your table view.

Assign your custom delegate object to the dropDelegate property of your table view.

## Topics

### Declaring support for handling drops

func tableView(UITableView, canHandle: any UIDropSession) -> Bool

Asks your delegate whether it can accept the specified type of data.

### Providing a custom drop preview

func tableView(UITableView, dropPreviewParametersForRowAt: IndexPath) -> UIDragPreviewParameters?

Returns custom information about how to display the row at the specified location during the drop.

### Incorporating the dropped data

func tableView(UITableView, performDropWith: any UITableViewDropCoordinator)

Incorporates the dropped data into your data structures and updates the table.

**Required**

### Tracking the drag movements

func tableView(UITableView, dropSessionDidUpdate: any UIDropSession, withDestinationIndexPath: IndexPath?) -> UITableViewDropProposal

Proposes how to handle a drop at the specified location in the table view.

func tableView(UITableView, dropSessionDidEnter: any UIDropSession)

Notifies the delegate when dragged content enters the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidExit: any UIDropSession)

Notifies the delegate when dragged content exits the table view’s bounds rectangle.

func tableView(UITableView, dropSessionDidEnd: any UIDropSession)

Notifies the delegate when the drag operation ends.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag and drop

Supporting drag and drop in table views

Initiate drags and handle drops from a table view.

Adopting drag and drop in a table view

Demonstrates how to enable and implement drag and drop for a table view.

protocol UITableViewDragDelegate

The interface for initiating drags from a table view.

protocol UITableViewDropCoordinator

An interface for coordinating your custom drop-related actions with the table view.

protocol UITableViewDropItem

The data associated with an item being dropped into the table view.

class UITableViewDropProposal

Your proposed solution for handling a drop in a table view.

