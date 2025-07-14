

- AppKit
-  NSCollectionViewDelegateFlowLayout 

Protocol

# NSCollectionViewDelegateFlowLayout

A set of methods that a delegate implements to provide layout information to a flow layout object in a collection view.

macOS

``` source
protocol NSCollectionViewDelegateFlowLayout : NSCollectionViewDelegate
```

## Overview

Implement the methods of this protocol when you want to customize the layout behavior and perhaps return different values for different items or sections.

All of the methods in this protocol are optional, so you can implement only the methods you need to achieve the desired layout. If you do not implement a particular method, the flow layout object obtains default values from its own properties and applies them uniformly. Implement your methods in the object you assign to the delegate property of the collection view itself.

## Topics

### Getting the Size of Items

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, sizeForItemAt: IndexPath) -> NSSize

Asks the delegate for the size of the specified item.

### Getting the Section Spacing

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, insetForSectionAt: Int) -> NSEdgeInsets

Asks the delegate for the margins to apply to content in the specified section.

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, minimumLineSpacingForSectionAt: Int) -> CGFloat

Asks the delegate for the spacing between successive rows or columns of a section.

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, minimumInteritemSpacingForSectionAt: Int) -> CGFloat

Asks the delegate for the spacing between successive items of a single row or column.

### Getting the Header and Footer Sizes

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, referenceSizeForHeaderInSection: Int) -> NSSize

Asks the delegate for the size of the header view in the specified section.

func collectionView(NSCollectionView, layout: NSCollectionViewLayout, referenceSizeForFooterInSection: Int) -> NSSize

Asks the delegate for the size of the footer view in the specified section.

## Relationships

### Inherits From

- NSCollectionViewDelegate
- NSObjectProtocol

## See Also

### Layouts

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

class NSCollectionViewFlowLayout

A layout that organizes items into a flexible and configurable arrangement.

class NSCollectionViewGridLayout

A layout that displays a single section of items in a row and column grid.

class NSCollectionViewTransitionLayout

An object that implements custom behaviors when changing from one layout to another in a collection view.

class NSCollectionViewLayoutAttributes

An object that contains layout-related attributes for an element in a collection view.

class NSCollectionViewLayout

An abstract base class that you subclass and use to generate layout information for a collection view.

class NSCollectionViewCompositionalLayout

A layout object that lets you combine items in highly adaptive and flexible visual arrangements.

class NSCollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

typealias NSCollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

enum NSCollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

