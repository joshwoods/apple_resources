

- AppKit
-  NSCollectionViewUpdateItem 

Class

# NSCollectionViewUpdateItem

A description of a single change to make to an item in a collection view.

macOS 10.11+

``` source
@MainActor
class NSCollectionViewUpdateItem
```

## Overview

You do not create instances of this class directly. When updating its content, the collection view object creates them and passes them to the layout object’s prepare(forCollectionViewUpdates:) method, which can use them to prepare for the upcoming changes.

## Topics

### Accessing the Item Changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var indexPathAfterUpdate: IndexPath?

The index path of the item after the update.

var updateAction: NSCollectionView.UpdateAction

The action being performed on the item.

enum UpdateAction

Constants indicating the type of action being performed on an item.

enum ScrollDirection

Constants indicating the scrolling direction for the layout.

### Constants

enum UpdateAction

Constants indicating the type of action being performed on an item.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Updates

class NSCollectionViewLayoutInvalidationContext

An object that identifies the portions of your layout that need to be updated.

class NSCollectionViewFlowLayoutInvalidationContext

An object that identifies the portions of a flow layout object that need to be updated.

