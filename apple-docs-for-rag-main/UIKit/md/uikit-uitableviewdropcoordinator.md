

- UIKit
-  UITableViewDropCoordinator 

Protocol

# UITableViewDropCoordinator

An interface for coordinating your custom drop-related actions with the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITableViewDropCoordinator : NSObjectProtocol
```

## Mentioned in 

Supporting drag and drop in table views

## Overview

Don’t create instances of this class yourself. When a drop occurs in the table view, UIKit creates an instance of this class and passes it to your tableView(_:performDropWith:) method. Use the object to let the table view know how you want to animate the dropped items into position.

## Topics

### Getting the dragged items

var items: [any UITableViewDropItem]

The items being dragged.

**Required**

### Getting the drop location

var destinationIndexPath: IndexPath?

The index path at which to insert the item into the table view.

**Required**

### Animating rows to their destination

func drop(UIDragItem, toRowAt: IndexPath) -> any UIDragAnimating

Animates the item to the specified index path in the table view.

**Required**

func drop(UIDragItem, intoRowAt: IndexPath, rect: CGRect) -> any UIDragAnimating

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

func drop(UIDragItem, to: UITableViewDropPlaceholder) -> any UITableViewDropPlaceholderContext

Animates the item to the specified location and inserts a placeholder cell at that location.

**Required**

### Getting the session information

var session: any UIDropSession

The drop session containing information about the transaction.

**Required**

var proposal: UITableViewDropProposal

The proposal for how to incorporate the dropped items.

**Required**

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

protocol UITableViewDropDelegate

The interface for handling drops in a table view.

protocol UITableViewDropItem

The data associated with an item being dropped into the table view.

class UITableViewDropProposal

Your proposed solution for handling a drop in a table view.

