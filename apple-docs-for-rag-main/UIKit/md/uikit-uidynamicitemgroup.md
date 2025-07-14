

- UIKit
-  UIDynamicItemGroup 

Class

# UIDynamicItemGroup

A dynamic item that comprises multiple other dynamic items.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIDynamicItemGroup
```

## Overview

Use groups to manipulate a group of dynamic items together and treat them as a single unit for the purpose of collisions. The group can contain dynamic items but cannot contain other UIDynamicItemGroup objects. You can add a group to any UIDynamicBehavior object.

The attributes of the dynamic item group are derived from the items of the group itself. The group’s bounds rectangle is the rectangle that encloses all of the contained dynamic items, and the center point of the group is the center point of the bounds rectangle.

## Topics

### Initializing a group

init(items: [any UIDynamicItem])

Initializes and returns a group containing the specified items.

### Getting the dynamic items in a group

var items: [any UIDynamicItem]

The dynamic items in the group.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIDynamicItem

## See Also

### Dynamic Items

protocol UIDynamicItem

A set of methods that can make a custom object eligible to participate in UIKit Dynamics.

class UIDynamicItemBehavior

A base dynamic animation configuration for one or more dynamic items.

