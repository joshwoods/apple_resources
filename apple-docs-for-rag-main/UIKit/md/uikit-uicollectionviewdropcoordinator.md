

- UIKit
-  UICollectionViewDropCoordinator 

Protocol

# UICollectionViewDropCoordinator

An interface for coordinating your custom drop-related actions with the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UICollectionViewDropCoordinator : NSObjectProtocol
```

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Overview

You don’t create instances of this class yourself. When a drop occurs in the collection view, UIKit creates an instance of this class and passes it to your collectionView(_:performDropWith:) method. Use the object to let the collection view know how you want to animate the dropped items into position.

## Topics

### Getting the Dragged Items

var items: [any UICollectionViewDropItem]

The items being dragged.

**Required**

### Getting the Drop Location

var destinationIndexPath: IndexPath?

The index path at which to insert the item in the collection view.

**Required**

### Animating Items to Their Destination

func drop(UIDragItem, toItemAt: IndexPath) -> any UIDragAnimating

Animates the item to the specified index path in the collection view.

**Required**

func drop(UIDragItem, intoItemAt: IndexPath, rect: CGRect) -> any UIDragAnimating

Animates the item to the specified rectangle in the collection view.

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

func drop(UIDragItem, to: UICollectionViewDropPlaceholder) -> any UICollectionViewDropPlaceholderContext

Animates the item to the specified location and inserts a placeholder cell at that location.

**Required**

### Getting the Session Information

var session: any UIDropSession

The drop session containing information about the transaction.

**Required**

var proposal: UICollectionViewDropProposal

The current proposal for how to incorporate the dropped items.

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

class UICollectionViewDropPlaceholder

A placeholder for an item dropped on a collection view.

class UICollectionViewDropProposal

Your proposed solution for handling a drop in a collection view.

protocol UICollectionViewDropItem

The data associated with an item being dropped into the collection view.

protocol UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

