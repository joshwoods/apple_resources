

- UIKit
- UIRegion
-  init(size:) 

Initializer

# init(size:)

Initializes and returns a rectangular region of the specified size.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(size: CGSize)
```

## Parameters 

`size`  

The size of the region, specified in points.

## Return Value

A rectangular region of the specified size.

## Discussion

The center of the rectangle is the origin of the region’s coordinate system.

## See Also

### Creating and initializing regions

class var infinite: UIRegion

Returns the region that encloses all points.

init(radius: CGFloat)

Initializes and returns a region with a circular shape of the specified radius.

