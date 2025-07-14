

- SwiftUI
- UnitPoint3D
-  origin 

Type Property

# origin

The origin of a view.

visionOS 1.0+

``` source
static let origin: UnitPoint3D
```

## Discussion

A view’s origin appears in the top-left-back corner in a left-to-right language environment, with positive x toward the right. It appears in the top-right-back corner in a right-to-left language, with positive x toward the left. Positive y is always toward the bottom of the view, and positive z points toward the front.

## See Also

### Getting the origin

static let zero: UnitPoint3D

A 3D unit point with all components equal to zero.

