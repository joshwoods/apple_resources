

- UIKit
-  UICollectionViewDropPlaceholderContext 

Protocol

# UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UICollectionViewDropPlaceholderContext : UIDragAnimating
```

## Overview

You do not create instances of this class yourself. For each placeholder cell that you insert into the collection view, the drop coordinator provides you with an instance of this class. You use this context object later to remove the placeholder cell, either by committing the actual data to your data source object or by deleting the placeholder cell.

## Topics

### Updating the Placeholder Cell

func commitInsertion(dataSourceUpdates: (IndexPath) -> Void) -> Bool

Exchanges the placeholder cell for a cell with the final content.

**Required**

func setNeedsCellUpdate()

Updates the contents of the placeholder cell.

**Required**

### Removing the Placeholder Cell

func deletePlaceholder() -> Bool

Removes an unneeded placeholder cell altogether from the collection view.

**Required**

### Getting the Drag Item

var dragItem: UIDragItem

The drag item being represented by the placeholder cell.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIDragAnimating

## See Also

### Drag and drop

Supporting Drag and Drop in Collection Views

Initiate drags and handle drops from a collection view.

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

protocol UICollectionViewDropDelegate

The interface for handling drops in a collection view.

protocol UICollectionViewDropCoordinator

An interface for coordinating your custom drop-related actions with the collection view.

class UICollectionViewDropPlaceholder

A placeholder for an item dropped on a collection view.

class UICollectionViewDropProposal

Your proposed solution for handling a drop in a collection view.

protocol UICollectionViewDropItem

The data associated with an item being dropped into the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

