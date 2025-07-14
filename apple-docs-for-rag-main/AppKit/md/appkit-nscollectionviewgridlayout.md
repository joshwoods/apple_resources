

- AppKit
-  NSCollectionViewGridLayout 

Class

# NSCollectionViewGridLayout

A layout that displays a single section of items in a row and column grid.

macOS 10.11+

``` source
@MainActor
class NSCollectionViewGridLayout
```

## Overview

The NSCollectionViewGridLayout object provides the same layout behavior offered by the NSCollectionView class prior to macOS 10.11, and you can use it in cases where you want to maintain the old appearance while still taking advantage of newer collection view features.

### Configuring a Collection View to Use a Grid Layout

You can configure a collection view to use a grid layout object programmatically or at design time:

- At design time, set the Layout attribute of your collection view to Grid.

- Create an `NSCollectionViewGridLayout` object programmatically and assign it to the collection view’s collectionViewLayout property.

A grid layout displays only items and does not display supplementary views or decoration views. Use the properties of this class to configure the number of rows and columns in the grid. You can also use these properties to configure the spacing between items and the minimum sizes.

## Topics

### Specifying the Grid Parameters

var maximumNumberOfRows: Int

The maximum number of rows to display in the collection view’s visible area.

var maximumNumberOfColumns: Int

The maximum number of columns to display in the collection view’s visible area.

var minimumItemSize: NSSize

The smallest allowable size for an item’s view.

var maximumItemSize: NSSize

The largest allowable size for an item’s view.

### Specifying the Grid Layout Attributes

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

var margins: NSEdgeInsets

The amount of empty space (in points) around the grid’s content.

### Specifying the Grid Background Color

var backgroundColors: [NSColor]!

The array of background colors to use when drawing the grid.

## Relationships

### Inherits From

- NSCollectionViewLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Layouts

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

class NSCollectionViewFlowLayout

A layout that organizes items into a flexible and configurable arrangement.

protocol NSCollectionViewDelegateFlowLayout

A set of methods that a delegate implements to provide layout information to a flow layout object in a collection view.

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

