

- UIKit
-  UITableViewDropItem 

Protocol

# UITableViewDropItem

The data associated with an item being dropped into the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITableViewDropItem : NSObjectProtocol
```

## Overview

When handling a drop, you get instances of this class from the items property of the UITableViewDropCoordinator object. Use them to retrieve the data for the items being dragged and to plan any animations related to dropping the items. You don’t create instances of this class yourself.

## Topics

### Getting the drag item

var dragItem: UIDragItem

The item that was dragged.

**Required**

### Getting the item information

var previewSize: CGSize

The size of the drag item’s preview.

**Required**

var sourceIndexPath: IndexPath?

The index path of the item in the table view, if any.

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

protocol UITableViewDropCoordinator

An interface for coordinating your custom drop-related actions with the table view.

class UITableViewDropProposal

Your proposed solution for handling a drop in a table view.

