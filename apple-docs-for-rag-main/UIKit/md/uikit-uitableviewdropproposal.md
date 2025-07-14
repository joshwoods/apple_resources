

- UIKit
-  UITableViewDropProposal 

Class

# UITableViewDropProposal

Your proposed solution for handling a drop in a table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITableViewDropProposal
```

## Mentioned in 

Supporting drag and drop in table views

## Overview

Create instances of this class in the tableView(_:dropSessionDidUpdate:withDestinationIndexPath:) method of your drop delegate object. You create drop proposals to let the table view know how you intend to handle a drop at the currently specified location. The table view uses that information to provide appropriate visual feedback to the user.

## Topics

### Creating a drop proposal

init(operation: UIDropOperation, intent: UITableViewDropProposal.Intent)

Creates a drop proposal object that specifies how to incorporate the dropped content.

### Getting the proposed drop location

var intent: UITableViewDropProposal.Intent

The option to use when incorporating dropped items into your content.

enum Intent

Constants indicating how you intend to handle a drop.

enum UIDropOperation

Operation types that determine how a drag and drop activity resolves when the user drops a drag item.

## Relationships

### Inherits From

- UIDropProposal

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

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

protocol UITableViewDropItem

The data associated with an item being dropped into the table view.

