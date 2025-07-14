

- TVUIKit
-  TVCollectionViewDelegateFullScreenLayout 

Protocol

# TVCollectionViewDelegateFullScreenLayout

Methods that send notifications of events during cell transitions.

tvOS 13.0+

``` source
protocol TVCollectionViewDelegateFullScreenLayout : UICollectionViewDelegate
```

## Overview

The methods contained in this protocol help you manage and control cell transitions.

## Topics

### Managing Cell Transitions

func collectionView(UICollectionView, layout: UICollectionViewLayout, willCenterCellAt: IndexPath)

Tells the delegate when a cell is to be the center cell.

func collectionView(UICollectionView, layout: UICollectionViewLayout, didCenterCellAt: IndexPath)

Tells the delegate when a cell has completed the transition and has become the center cell.

## Relationships

### Inherits From

- NSObjectProtocol
- UICollectionViewDelegate
- UIScrollViewDelegate

## See Also

### Collections of content

Creating immersive experiences using a full-screen layout

Display content with a collection view that maximizes the tvOS experience.

class TVCollectionViewFullScreenLayout

A collection view layout that organizes items into a browsable, full-screen display format.

class TVCollectionViewFullScreenCell

A full-screen cell to use in full-screen display format.

class TVCollectionViewFullScreenLayoutAttributes

Attributes to manage the appearance of the collection view’s layout.

