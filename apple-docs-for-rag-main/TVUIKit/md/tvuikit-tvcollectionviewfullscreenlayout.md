

- TVUIKit
-  TVCollectionViewFullScreenLayout 

Class

# TVCollectionViewFullScreenLayout

A collection view layout that organizes items into a browsable, full-screen display format.

tvOS 13.0+

``` source
@MainActor
class TVCollectionViewFullScreenLayout
```

## Overview

Use this class to create a full-screen browsing experience. Full-screen layouts are an immersive way to present and navigate through content.

## Topics

### Managing a collection view’s appearance

var interitemSpacing: CGFloat

The spacing between each cell in a collection view.

### Accessing collection view items

var centerIndexPath: IndexPath?

The index path of the currently centered item.

### Configuring cell masks

var maskAmount: CGFloat

The amount by which to mask the cells in a collection view.

var maskInset: UIEdgeInsets

The edge insets of the cell mask.

### Managing cell appearance

var cornerRadius: CGFloat

The radius to use when drawing rounded corners for the cell.

### Managing transitions

var parallaxFactor: CGFloat

A value that specifies how slowly the background should move relative to the foreground.

var isTransitioningToCenterIndexPath: Bool

A Boolean value that indicates whether the cell is changing index paths.

## Relationships

### Inherits From

- UICollectionViewLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Collections of content

Creating immersive experiences using a full-screen layout

Display content with a collection view that maximizes the tvOS experience.

protocol TVCollectionViewDelegateFullScreenLayout

Methods that send notifications of events during cell transitions.

class TVCollectionViewFullScreenCell

A full-screen cell to use in full-screen display format.

class TVCollectionViewFullScreenLayoutAttributes

Attributes to manage the appearance of the collection view’s layout.

