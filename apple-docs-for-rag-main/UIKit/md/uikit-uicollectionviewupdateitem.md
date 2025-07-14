

- UIKit
-  UICollectionViewUpdateItem 

Class

# UICollectionViewUpdateItem

An object that describes a single change to make to an item in a collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UICollectionViewUpdateItem
```

## Overview

You don’t create instances of this class directly. When updating its content, the collection view object creates them and passes them to the layout object’s prepare(forCollectionViewUpdates:) method, which can use them to prepare the layout object for the upcoming changes.

## Topics

### Accessing the item changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var indexPathAfterUpdate: IndexPath?

The index path of the item after the update.

var updateAction: UICollectionViewUpdateItem.Action

The action being performed on the item.

enum Action

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

### Layout updates

protocol NSCollectionLayoutVisibleItem

An item that’s currently visible within the bounds of a section.

typealias NSCollectionLayoutSectionVisibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of items in a section immediately before they’re displayed.

class UICollectionViewFocusUpdateContext

A context object that stores information specific to a focus update in a collection view.

class UICollectionViewLayoutInvalidationContext

A context object that declares which parts of your layout need to be updated when the layout is invalidated.

