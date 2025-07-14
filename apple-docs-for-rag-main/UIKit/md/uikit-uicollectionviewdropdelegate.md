

- UIKit
-  UICollectionViewDropDelegate 

Protocol

# UICollectionViewDropDelegate

The interface for handling drops in a collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UICollectionViewDropDelegate : NSObjectProtocol
```

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Overview

Implement this protocol in the object that you use to incorporate dropped data into your collection view. The only required method of this protocol is the collectionView(_:performDropWith:) method, but you can implement other methods as needed to customize the drop behavior of your collection view.

Assign your custom delegate object to the dropDelegate property of your collection view.

## Topics

### Declaring support for handling drops

func collectionView(UICollectionView, canHandle: any UIDropSession) -> Bool

Asks your delegate whether the collection view can accept a drop with the specified type of data.

### Incorporating the dropped data

func collectionView(UICollectionView, performDropWith: any UICollectionViewDropCoordinator)

Tells your delegate to incorporate the drop data into the collection view.

**Required**

### Tracking the drag movements

func collectionView(UICollectionView, dropSessionDidUpdate: any UIDropSession, withDestinationIndexPath: IndexPath?) -> UICollectionViewDropProposal

Tells your delegate that the position of the dragged data over the collection view changed.

func collectionView(UICollectionView, dropSessionDidEnter: any UIDropSession)

Notifies you when dragged content enters the collection view’s bounds rectangle.

func collectionView(UICollectionView, dropSessionDidExit: any UIDropSession)

Notifies you when dragged content exits the collection view’s bounds rectangle.

func collectionView(UICollectionView, dropSessionDidEnd: any UIDropSession)

Notifies you when the drag operation ends.

### Providing a custom preview

func collectionView(UICollectionView, dropPreviewParametersForItemAt: IndexPath) -> UIDragPreviewParameters?

Returns custom information about how to display the item at the specified location during the drop.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag and drop

Supporting Drag and Drop in Collection Views

Initiate drags and handle drops from a collection view.

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

protocol UICollectionViewDropCoordinator

An interface for coordinating your custom drop-related actions with the collection view.

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

