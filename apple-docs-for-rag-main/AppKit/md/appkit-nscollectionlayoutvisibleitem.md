

- AppKit
-  NSCollectionLayoutVisibleItem 

Protocol

# NSCollectionLayoutVisibleItem

An item that’s currently visible within the bounds of a section.

macOS 10.15+

``` source
@MainActor
protocol NSCollectionLayoutVisibleItem : NSObjectProtocol
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

var representedElementCategory: NSCollectionElementCategory

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

var frame: NSRect

The frame rectangle, which describes the item’s location and size in its section’s coordinate system.

**Required**

var bounds: NSRect

The bounds rectangle, which describes the item’s location and size in its own coordinate system.

**Required**

var center: NSPoint

The center point of the item’s frame rectangle.

**Required**

### Specifying stacking order

var zIndex: Int

The vertical stacking order of the item in relation to other items in the section.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Layout updates

typealias NSCollectionLayoutSectionVisibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of items in a section immediately before they’re displayed.

