

- UIKit
-  UICollectionViewPlaceholder 

Class

# UICollectionViewPlaceholder

A placeholder for an item dragged or dropped on a collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UICollectionViewPlaceholder
```

## Topics

### Initializing a Placeholder

init(insertionIndexPath: IndexPath, reuseIdentifier: String)

Creates a placeholder object with the specified index path and reuse identifier.

### Updating the Cell’s Content

var cellUpdateHandler: ((UICollectionViewCell) -> Void)?

The block that updates the contents of the placeholder cell.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UICollectionViewDropPlaceholder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

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

protocol UICollectionViewDropPlaceholderContext

An object that contains information about a placeholder in the collection view.

protocol UIDataSourceTranslating

An advanced interface for managing a data source object.

