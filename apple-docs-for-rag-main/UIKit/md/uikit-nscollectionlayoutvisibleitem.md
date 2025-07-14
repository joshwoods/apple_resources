

- UIKit
-  NSCollectionLayoutVisibleItem 

Protocol

# NSCollectionLayoutVisibleItem

An item that’s currently visible within the bounds of a section.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol NSCollectionLayoutVisibleItem : UIDynamicItem
```

## Overview

A visible item represents an item in a collection view that’s currently visible onscreen, such as a cell, supplementary view, or decoration. You access a specific section’s visible items in its visible item invalidation handler (NSCollectionLayoutSectionVisibleItemsInvalidationHandler), stored in the visibleItemsInvalidationHandler property. The handler is called before each layout cycle, any time an animation occurs in that section due to changes such as adding or removing items, scrolling the section, or rotating the device.

## Topics

### Identifying the item

var name: String

The name of the item.

**Required**

var representedElementKind: String?

A string that identifies the type of item.

**Required**

var representedElementCategory: UICollectionView.ElementCategory

A category that identifies the item, such as decoration or supplementary view.

**Required**

### Getting the index path

var indexPath: IndexPath

The index path of the item.

**Required**

### Configuring appearance

var alpha: CGFloat

The transparency of the item.

**Required**

var isHidden: Bool

A Boolean value that determines whether the item is hidden.

**Required**

### Configuring position

var frame: CGRect

The frame rectangle, which describes the item’s location and size in its section’s coordinate system.

**Required**

var bounds: CGRect

The bounds rectangle, which describes the item’s location and size in its own coordinate system.

**Required**

var center: CGPoint

The center point of the item’s frame rectangle.

**Required**

var transform: CGAffineTransform

The transform applied to the item, relative to the center of its bounds.

**Required**

var transform3D: CATransform3D

The 3D transform applied to the item.

**Required**

### Specifying stacking order

var zIndex: Int

The vertical stacking order of the item in relation to other items in the section.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIDynamicItem

## See Also

### Layout updates

typealias NSCollectionLayoutSectionVisibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of items in a section immediately before they’re displayed.

class UICollectionViewUpdateItem

An object that describes a single change to make to an item in a collection view.

class UICollectionViewFocusUpdateContext

A context object that stores information specific to a focus update in a collection view.

class UICollectionViewLayoutInvalidationContext

A context object that declares which parts of your layout need to be updated when the layout is invalidated.

