

- SpriteKit
- SKShapeNode
-  init(splinePoints:count:) 

Initializer

# init(splinePoints:count:)

Creates a shape node from a series of spline points.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
convenience init(
    splinePoints points: UnsafeMutablePointer,
    count numPoints: Int
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    splinePoints points: UnsafeMutablePointer,
    count numPoints: Int
)
```

## Parameters 

`points`  

An array of Core Graphics points.

`numPoints`  

The number of points in the array.

## Return Value

A new shape node is created. The node is created with a path that starts at the first point in the array, joining each pair of points with a quadratic curve. The control points are calculated automatically based on previous points in the array.

## Mentioned in 

Creating a Shape Node from an Array of Points

## See Also

### Creating a Shape from an Array of Points

Creating a Shape Node from an Array of Points

Create jagged or smooth shapes from the same array of points.

convenience init(points: UnsafeMutablePointer&lt;CGPoint>, count: Int)

Creates a shape node from a series of points.

