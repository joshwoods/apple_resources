

- SwiftUI
- UnitPoint3D
-  init(x:y:z:) 

Initializer

# init(x:y:z:)

Creates a 3D unit point with the specified offsets.

visionOS 1.0+

``` source
init(
    x: CGFloat,
    y: CGFloat,
    z: CGFloat
)
```

## Parameters 

`x`  

The normalized distance from the origin to the point in the horizontal dimension.

`y`  

The normalized distance from the origin to the point in the vertical dimension.

`z`  

The normalized distance from the origin to the point in the depth dimension.

## Discussion

Values outside the range `[0, 1]` project to points outside of a view.

## See Also

### Creating a point

init()

Creates a 3D unit point at the origin.

