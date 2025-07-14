

- UIKit
-  UICollectionViewDragDelegate 

Protocol

# UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UICollectionViewDragDelegate : NSObjectProtocol
```

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Overview

Implement this protocol in the object that you use to initiate drags from your collection view. The only required method of this protocol is the collectionView(_:itemsForBeginning:at:) method, but you can implement other methods as needed to customize the drag behavior of your collection view.

Assign your custom delegate object to the dragDelegate property of your collection view.

## Topics

### Providing the items to drag

func collectionView(UICollectionView, itemsForBeginning: any UIDragSession, at: IndexPath) -> [UIDragItem]

Provides the initial set of items (if any) to drag.

**Required**

func collectionView(UICollectionView, itemsForAddingTo: any UIDragSession, at: IndexPath, point: CGPoint) -> [UIDragItem]

Adds the specified items to an existing drag session.

### Tracking the drag session

func collectionView(UICollectionView, dragSessionWillBegin: any UIDragSession)

Notifies you that a drag session is about to begin for the collection view.

func collectionView(UICollectionView, dragSessionDidEnd: any UIDragSession)

Notifies you that a drag session ended for the collection view.

### Providing a custom preview

func collectionView(UICollectionView, dragPreviewParametersForItemAt: IndexPath) -> UIDragPreviewParameters?

Returns custom information about how to display the item at the specified location during the drag.

### Controlling the drag session

func collectionView(UICollectionView, dragSessionAllowsMoveOperation: any UIDragSession) -> Bool

Returns a Boolean value that determines whether a move operation is allowed for a drag session.

func collectionView(UICollectionView, dragSessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Returns a Boolean value that determines whether the source app and destination app must be the same for a drag session.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag and drop

Supporting Drag and Drop in Collection Views

Initiate drags and handle drops from a collection view.

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

protocol UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

