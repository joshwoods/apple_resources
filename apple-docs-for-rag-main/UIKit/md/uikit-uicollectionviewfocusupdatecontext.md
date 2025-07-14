

- UIKit
-  UICollectionViewFocusUpdateContext 

Class

# UICollectionViewFocusUpdateContext

A context object that stores information specific to a focus update in a collection view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UICollectionViewFocusUpdateContext
```

## Overview

When focus changes, the collection view delegate receives a context object with the relevant information. Your delegate methods use the information in this object to create animations or to perform other tasks related to the change in focus.

## Topics

### Locating focusable items in the collection view

var previouslyFocusedIndexPath: IndexPath?

The index path of the collection view cell that previously had the focus.

var nextFocusedIndexPath: IndexPath?

The index path of the collection view cell that’s receiving the focus.

## Relationships

### Inherits From

- UIFocusUpdateContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Layout updates

protocol NSCollectionLayoutVisibleItem

An item that’s currently visible within the bounds of a section.

typealias NSCollectionLayoutSectionVisibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of items in a section immediately before they’re displayed.

class UICollectionViewUpdateItem

An object that describes a single change to make to an item in a collection view.

class UICollectionViewLayoutInvalidationContext

A context object that declares which parts of your layout need to be updated when the layout is invalidated.

