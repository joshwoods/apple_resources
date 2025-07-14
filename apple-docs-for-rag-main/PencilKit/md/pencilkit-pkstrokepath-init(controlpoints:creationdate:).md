

- PencilKit
- PKStrokePath
-  init(controlPoints:creationDate:) 

Initializer

# init(controlPoints:creationDate:)

Creates a stroke path with the cubic B-spline control points and a date that you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    controlPoints: T,
    creationDate: Date
) where T : Sequence, T.Element == PKStrokePoint
```

## Parameters 

`controlPoints`  

An array of control points for a cubic B-spline.

`creationDate`  

The creation time of this path. The `timeOffset` of points in this stroke path is relative to this date.

## See Also

### Creating a new stroke path

init()

Creates an empty stroke path.

