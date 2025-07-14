

- SwiftUI
- UnitPoint3D
-  init() 

Initializer

# init()

Creates a 3D unit point at the origin.

visionOS 1.0+

``` source
init()
```

## Discussion

A view’s origin appears in the top-left-back corner in a left-to-right language environment, with positive x toward the right. It appears in the top-right-back corner in a right-to-left language, with positive x toward the left. Positive y is always toward the bottom of the view, and positive z points toward the front.

## See Also

### Creating a point

init(x: CGFloat, y: CGFloat, z: CGFloat)

Creates a 3D unit point with the specified offsets.

