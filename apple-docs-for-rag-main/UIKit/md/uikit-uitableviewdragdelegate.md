

- UIKit
-  UITableViewDragDelegate 

Protocol

# UITableViewDragDelegate

The interface for initiating drags from a table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITableViewDragDelegate : NSObjectProtocol
```

## Mentioned in 

Supporting drag and drop in table views

## Overview

Implement this protocol in the object that you use to initiate drags from your table view. The only required method of this protocol is the tableView(_:itemsForBeginning:at:) method, but you can implement other methods as needed to customize the drag behavior of your table view.

Assign your custom delegate object to the dragDelegate property of your table view.

## Topics

### Providing the items to drag

func tableView(UITableView, itemsForBeginning: any UIDragSession, at: IndexPath) -> [UIDragItem]

Provides the initial set of items (if any) to drag.

**Required**

func tableView(UITableView, itemsForAddingTo: any UIDragSession, at: IndexPath, point: CGPoint) -> [UIDragItem]

Adds the specified items to an existing drag session.

### Tracking the drag session

func tableView(UITableView, dragSessionWillBegin: any UIDragSession)

Signals the start of a drag operation involving content from the specified table view.

func tableView(UITableView, dragSessionDidEnd: any UIDragSession)

Signals the end of a drag operation involving content from the specified table view.

func tableView(UITableView, dragSessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Returns a Boolean value indicating whether the dragged content must be dropped in the same app.

func tableView(UITableView, dragSessionAllowsMoveOperation: any UIDragSession) -> Bool

Returns a Boolean value indicating whether your app supports a move operation for the dragged content.

### Providing a custom preview

func tableView(UITableView, dragPreviewParametersForRowAt: IndexPath) -> UIDragPreviewParameters?

Returns custom information about how to display the row at the specified location during the drag.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag and drop

Supporting drag and drop in table views

Initiate drags and handle drops from a table view.

Adopting drag and drop in a table view

Demonstrates how to enable and implement drag and drop for a table view.

protocol UITableViewDropDelegate

The interface for handling drops in a table view.

protocol UITableViewDropCoordinator

An interface for coordinating your custom drop-related actions with the table view.

protocol UITableViewDropItem

The data associated with an item being dropped into the table view.

class UITableViewDropProposal

Your proposed solution for handling a drop in a table view.

