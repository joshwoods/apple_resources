

- UIKit
- UIRegion
-  init(radius:) 

Initializer

# init(radius:)

Initializes and returns a region with a circular shape of the specified radius.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(radius: CGFloat)
```

## Parameters 

`radius`  

The radius of the circular area, specified in points.

## Return Value

A circular region with the specified radius.

## Discussion

The center of the circle is the origin of the region’s coordinate system.

## See Also

### Creating and initializing regions

class var infinite: UIRegion

Returns the region that encloses all points.

init(size: CGSize)

Initializes and returns a rectangular region of the specified size.

