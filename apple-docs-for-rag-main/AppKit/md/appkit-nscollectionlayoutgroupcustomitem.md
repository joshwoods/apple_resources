

- AppKit
-  NSCollectionLayoutGroupCustomItem 

Class

# NSCollectionLayoutGroupCustomItem

An item used in a group with a custom layout arrangement.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutGroupCustomItem
```

## Overview

You use a custom item if you want to specify a layout with a custom arrangement, like a radial or diagonal layout. You use custom items within a group that’s created with custom(layoutSize:itemProvider:).

Instead of providing a layout size for the custom item, like you do when you create an NSCollectionLayoutItem, you provide a frame instead.

## Topics

### Creating a custom item

convenience init(frame: NSRect)

Creates a custom item with the specified frame.

convenience init(frame: NSRect, zIndex: Int)

Creates a custom item with the specified frame and vertical stacking order in relation to other items in the group.

### Getting the frame

var frame: NSRect

The frame of the custom item.

### Specifying stacking order

var zIndex: Int

The vertical stacking order of the custom item in relation to other items in the group.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Advanced layouts

typealias NSCollectionLayoutGroupCustomItemProvider

A closure that creates and returns each of the custom group’s items.

