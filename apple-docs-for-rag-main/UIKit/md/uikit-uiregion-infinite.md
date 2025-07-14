

- UIKit
- UIRegion
-  infinite 

Type Property

# infinite

Returns the region that encloses all points.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class var infinite: UIRegion { get }
```

## Return Value

A shared region object that encompasses an infinite area.

## See Also

### Creating and initializing regions

init(size: CGSize)

Initializes and returns a rectangular region of the specified size.

init(radius: CGFloat)

Initializes and returns a region with a circular shape of the specified radius.

