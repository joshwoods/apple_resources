

- UIKit
- UIPencilHoverPose
-  azimuthUnitVector 

Instance Property

# azimuthUnitVector

A value that represents the azimuth unit vector of Apple Pencil in the specified view.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
var azimuthUnitVector: CGVector { get }
```

## See Also

### Getting the hover characteristics

var location: CGPoint

The location of an Apple Pencil above the view’s bounds, in view’s coordinate space.

var altitudeAngle: CGFloat

A value that represents the altitude angle of Apple Pencil.

var azimuthAngle: CGFloat

A value that represents the azimuth angle of Apple Pencil.

var rollAngle: CGFloat

A value that represents the barrel-roll angle of Apple Pencil.

var zOffset: CGFloat

A value that represents the normalized distance between the screen and Apple Pencil.

