

- UIKit
- NSCollectionLayoutVisibleItem
-  bounds 

Instance Property

# bounds

The bounds rectangle, which describes the item’s location and size in its own coordinate system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var bounds: CGRect { get }
```

**Required**

## See Also

### Configuring position

var frame: CGRect

The frame rectangle, which describes the item’s location and size in its section’s coordinate system.

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

