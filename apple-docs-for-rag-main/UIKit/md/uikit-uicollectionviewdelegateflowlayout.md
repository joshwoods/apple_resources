

- UIKit
-  UICollectionViewDelegateFlowLayout 

Protocol

# UICollectionViewDelegateFlowLayout

The methods that let you coordinate with a flow layout object to implement a grid-based layout.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UICollectionViewDelegateFlowLayout : UICollectionViewDelegate
```

## Overview

The methods of this protocol define the size of items and the spacing between items in the grid. All of the methods in this protocol are optional. If you don’t implement a particular method, the flow layout delegate uses values in its own properties for the appropriate spacing information.

The UICollectionViewFlowLayout object expects the collection view’s delegate object to adopt this protocol. Therefore, implement this protocol on the object assigned to your collection view’s delegate property.

## Topics

### Getting the size of items

func collectionView(UICollectionView, layout: UICollectionViewLayout, sizeForItemAt: IndexPath) -> CGSize

Asks the delegate for the size of the specified item’s cell.

### Getting the section spacing

func collectionView(UICollectionView, layout: UICollectionViewLayout, insetForSectionAt: Int) -> UIEdgeInsets

Asks the delegate for the margins to apply to content in the specified section.

func collectionView(UICollectionView, layout: UICollectionViewLayout, minimumLineSpacingForSectionAt: Int) -> CGFloat

Asks the delegate for the spacing between successive rows or columns of a section.

func collectionView(UICollectionView, layout: UICollectionViewLayout, minimumInteritemSpacingForSectionAt: Int) -> CGFloat

Asks the delegate for the spacing between successive items in the rows or columns of a section.

### Getting the header and footer sizes

func collectionView(UICollectionView, layout: UICollectionViewLayout, referenceSizeForHeaderInSection: Int) -> CGSize

Asks the delegate for the size of the header view in the specified section.

func collectionView(UICollectionView, layout: UICollectionViewLayout, referenceSizeForFooterInSection: Int) -> CGSize

Asks the delegate for the size of the footer view in the specified section.

## Relationships

### Inherits From

- NSObjectProtocol
- UICollectionViewDelegate
- UIScrollViewDelegate

