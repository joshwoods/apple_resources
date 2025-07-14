

- UIKit
-  UICollectionViewDropProposal 

Class

# UICollectionViewDropProposal

Your proposed solution for handling a drop in a collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UICollectionViewDropProposal
```

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Overview

Create instances of this class in the collectionView(_:dropSessionDidUpdate:withDestinationIndexPath:) method of your drop delegate object. You create drop proposals to let the collection view know how you intend to handle a drop at the currently specified location. The collection view uses that information to provide appropriate visual feedback to the user.

## Topics

### Creating a Drop Proposal

init(operation: UIDropOperation, intent: UICollectionViewDropProposal.Intent)

Creates a drop proposal object that specifies how to incorporate the dropped content.

### Getting the Proposed Drop Location

var intent: UICollectionViewDropProposal.Intent

The option to use when incorporating the dropped items into your content.

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

protocol UICollectionViewDropItem

The data associated with an item being dropped into the collection view.

protocol UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

class UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

