

- SwiftUI
- UnitPoint
-  init(x:y:) 

Initializer

# init(x:y:)

Creates a unit point with the specified horizontal and vertical offsets.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    x: CGFloat,
    y: CGFloat
)
```

## Parameters 

`x`  

The normalized distance from the origin to the point in the horizontal direction.

`y`  

The normalized distance from the origin to the point in the vertical direction.

## Discussion

Values outside the range `[0, 1]` project to points outside of a view.

## See Also

### Creating a point

init()

Creates a unit point at the origin.

