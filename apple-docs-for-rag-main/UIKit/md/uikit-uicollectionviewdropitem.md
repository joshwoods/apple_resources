

- UIKit
-  UICollectionViewDropItem 

Protocol

# UICollectionViewDropItem

The data associated with an item being dropped into the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UICollectionViewDropItem : NSObjectProtocol
```

## Overview

When handling a drop, you get instances of this class from the items property of the UICollectionViewDropCoordinator object. Use them to retrieve the data for the items being dragged and to plan any animations related to dropping the items. You do not create instances of this class yourself.

## Topics

### Getting the Drag Item

var dragItem: UIDragItem

The item that was dragged.

**Required**

### Getting the Item Information

var previewSize: CGSize

The size of the drag item’s preview.

**Required**

var sourceIndexPath: IndexPath?

The index path of the item in the collection view, if any.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

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

protocol UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

