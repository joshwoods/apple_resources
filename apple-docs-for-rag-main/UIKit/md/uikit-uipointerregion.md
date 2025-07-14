

- UIKit
-  UIPointerRegion 

Class

# UIPointerRegion

A rectangular region that interacts with pointer movements.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class UIPointerRegion
```

## Topics

### Creating a region

convenience init(rect: CGRect, identifier: AnyHashable?)

Creates a pointer region with the specified rectangle and optional identifier.

### Configuring a region

var rect: CGRect

The rectangle bounds of the region.

var identifier: AnyHashable?

An optional identifier for the region.

var latchingAxes: UIAxis

Axes along which the region latches after a primary click.

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

### Pointer region

class UIPointerRegionRequest

An object to describe the pointer’s location in the interaction’s view.

